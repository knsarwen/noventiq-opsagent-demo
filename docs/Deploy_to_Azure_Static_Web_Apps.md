# Deploying Noventiq OpsAgent Demo HUD to Azure Static Web Apps

This guide explains how to deploy the **Noventiq OpsAgent Hotel Domain Control Center** to **Azure Static Web Apps (Free Tier)** so that all booth presenters can access the live web application URL from any device.

---

## 🚀 Option A: Deploy via Azure Portal (Simplest & Fast - 3 Minutes)

### Prerequisites:
- Access to an Azure Subscription (or your Visual Studio Enterprise Azure Sponsorship / Partner Sandbox).
- A GitHub repository containing the files in `c:\Users\kumarsl\OneDrive - Noventiq Holdings PLC\Desktop\UOB`.

### Step-by-Step Instructions:
1. **Push Code to GitHub**:
   - Push `index.html`, `styles.css`, `app.js`, and `staticwebappconfig.json` to a public or private GitHub repository (e.g. `Noventiq-OpsAgent-Demo`).

2. **Create Azure Static Web App Resource**:
   - Sign in to the [Azure Portal](https://portal.azure.com/).
   - Click **+ Create a resource** $\rightarrow$ Search for **Static Web App** $\rightarrow$ Click **Create**.
   - Fill in the details:
     - **Subscription**: Your Azure Sponsorship / Partner Subscription
     - **Resource Group**: `rg-noventiq-opsagent-demo`
     - **Name**: `noventiq-opsagent-hud`
     - **Plan Type**: **Free** ($0.00 / month)
     - **Region**: East Asia or Southeast Asia
   - Under **Deployment Details**:
     - Select **GitHub** as the source.
     - Authorize your GitHub account and select your repository & branch (`main`).
     - Under **Build Presets**: Select **Custom**.
     - **App location**: `/`
     - **Api location**: *(leave empty)*
     - **Output location**: `/`
   - Click **Review + create** $\rightarrow$ Click **Create**.

3. **Get Live Booth URL**:
   - Once deployment completes (~1 minute), go to the resource page in Azure Portal.
   - Copy the generated **URL** (e.g., `https://nice-ocean-0a1234567.azurestaticapps.net`).
   - Share this link with all booth presenters!

---

## ⚡ Option B: Deploy via Azure CLI (Command Line)

If Azure CLI & SWA CLI are installed on your machine, run:

```powershell
# 1. Login to Azure
az login

# 2. Create Resource Group
az group create --name rg-noventiq-opsagent-demo --location southeastasia

# 3. Create Static Web App
az staticwebapp create `
  --name noventiq-opsagent-hud `
  --resource-group rg-noventiq-opsagent-demo `
  --location southeastasia `
  --sku Free

# 4. Deploy static files using SWA CLI
npx @azure/static-web-apps-cli deploy ./ --env production
```

---

## 📱 Local Access (Offline Backup at the Booth)

If internet connection at the booth drops, presenters can open the standalone file directly in any browser:
- Open file: [`index.html`](file:///c:/Users/kumarsl/OneDrive%20-%20Noventiq%20Holdings%20PLC/Desktop/UOB/index.html)
- Works 100% offline with zero dependencies!

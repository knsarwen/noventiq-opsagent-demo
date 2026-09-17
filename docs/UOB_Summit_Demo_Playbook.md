# UOB Summit: Noventiq Microsoft Partner Presentation & Live Demo Playbook

**Session Title**: The Pragmatic 3-6-5 AI Playbook for Capital-Efficient AI Capabilities  
**Subtitle**: *No custom code, no multi-million-dollar budgets—how regional SMEs operationalize Microsoft M365 & Copilot Studio across 3 Phases, 6 Weeks, and 5 Universal Capabilities.*  
**Presenter / Partner**: Noventiq Solutions (Microsoft Solution Partner)  

---

## 🎯 Summit Objectives & Key Message

At the UOB Summit, Noventiq demonstrates how regional SMEs can break through **"The Copilot Wall"**. Rather than pitch expensive, custom AI science projects, Noventiq shows how to leverage the customer's existing **Microsoft 365, Copilot Studio, and Power Platform** licenses to turn multi-day operational bottlenecks into **30-second decisions**.

---

## 📊 Presentation Deck Structure & Narrative

```
+-----------------------------------------------------------------------------------+
|                           SLIDE 1: THE 3-6-5 HOOK                                 |
|          "Stop buying AI science projects. Activate your M365 stack."              |
+-----------------------------------------+-----------------------------------------+
                                          |
                                          v
+-----------------------------------------------------------------------------------+
|                        SLIDE 2: WHY SME AI PROJECTS FAIL                          |
|             "Siloed tools, vendor lock-in, custom code maintenance"              |
+-----------------------------------------+-----------------------------------------+
                                          |
                                          v
+-----------------------------------------------------------------------------------+
|                    SLIDE 3: THE 5 UNIVERSAL CAPABILITIES                          |
|               Understand -> Connect -> Generate -> Govern -> Execute              |
+-----------------------------------------+-----------------------------------------+
                                          |
                                          v
+-----------------------------------------------------------------------------------+
|                   SLIDE 4: LOW-CODE ARCHITECTURE UNDERNEATH                       |
|           Copilot Studio + Power Automate + Dataverse / Fabric OneLake            |
+-----------------------------------------+-----------------------------------------+
                                          |
                                          v
+-----------------------------------------------------------------------------------+
|                    SLIDE 5: LIVE DEMO (NOVENTIQ OPSAGENT)                         |
|     Scenario A: B2B Quote Approval | Scenario B: Warranty Claim & Vision Triage   |
+-----------------------------------------+-----------------------------------------+
                                          |
                                          v
+-----------------------------------------------------------------------------------+
|                    SLIDE 6: THE 3 PHASES IN 6 WEEKS ROADMAP                       |
|         Phase 1: Hygiene (W1-2) | Phase 2: Connect (W3-4) | Phase 3: Rollout (W5-6)  |
+-----------------------------------------------------------------------------------+
```

---

## 🎬 Live Demo Storyboard: Noventiq OpsAgent in Action

### Demo Scenario 1: Inquiry-to-Quotation (B2B Order Processing)
*Goal: Show how an unformatted PDF customer request turns into a 30-second automated quotation & approval.*

1. **Ingest (UNDERSTAND)**:
   - **Action**: Drop an unformatted customer RFP / PO PDF into an Outlook inbox or Teams channel.
   - **Screen**: Show Copilot Studio triggering **Azure AI Document Intelligence**, extracting line items, requested quantities, delivery timelines, and requested discounts in real-time.
2. **System Check & Pricing (CONNECT & GENERATE)**:
   - **Action**: OpsAgent queries Dataverse / Fabric OneLake customer ledgers for credit status and multi-currency exchange rates.
   - **Screen**: Power Automate fetches supplier unit cost & inventory lead time via ERP connector, then compiles a formatted quote PDF.
3. **1-Click Governance (GOVERN & EXECUTE)**:
   - **Action**: OpsAgent posts an **Adaptive Card (v1.5)** to Teams channel `#Sales-Finance-Approvals` tagging the Finance Lead.
   - **Screen**: Finance Lead clicks **[Approve Quote]**. OpsAgent instantly drafts/dispatches the final PDF quote via Outlook and logs the transaction in the ledger.

---

### Demo Scenario 2: After-Sales Warranty & Technical Vision Triage
*Goal: Show how an equipment defect photo + invoice photo yields an AI diagnostic score & stock reservation.*

1. **Claim Ingestion & Vision Triage (UNDERSTAND & CONNECT)**:
   - **Action**: Customer submits a warranty claim email with a photo of a damaged component and a tax invoice receipt.
   - **Screen**: Copilot Studio uses **Azure AI Document Intelligence** for receipt text, and **Azure OpenAI GPT-4o Vision** analyzes the defect photo.
   - **Result Displayed**: *"Technical Validity Score: 95% Valid Manufacturing Defect (Thermal Crack Pattern Identified)."*
2. **Stock Reservation & Finance Approval (GENERATE, GOVERN & EXECUTE)**:
   - **Action**: OpsAgent checks regional warehouse stock in Fabric/SQL and places a temporary stock reservation for the replacement part.
   - **Screen**: An Adaptive Card pops up for the Finance Manager displaying the credit note value, tax/shipping adjustments, and replacement cost.
   - **Click**: **[Authorize Credit Note & Dispatch Replacement]** automatically updates ERP and emails customer confirmation.

---

## 🛠️ Microsoft Stack Technical Architecture Highlights

| Capability Pillar | Microsoft Stack Component | Key Value Delivered |
| :--- | :--- | :--- |
| **Orchestration Core** | **Copilot Studio** | Unified conversational & event-driven agent core; zero code maintenance. |
| **1. Understand** | **Azure AI Document Intelligence** & **Azure OpenAI GPT-4o Vision** | Zero-template OCR table extraction & visual defect diagnosis. |
| **2. Connect** | **Power Automate** + **Microsoft Fabric OneLake / Dataverse** | Seamless connection across ERP, SQL, and enterprise data ledgers. |
| **3. Generate** | **Power Automate PDF Engine** | Automated branded proposal & credit note creation. |
| **4. Govern** | **Teams Adaptive Cards v1.5** | 1-click cross-functional approval with full audit trail. |
| **5. Execute** | **Outlook Integration & Dataverse Audit** | Automated customer dispatch & real-time financial ledger updates. |

---

## 🚀 Noventiq Booth Conversion Strategy

- **Interactive Sandbox**: Attendees can test dropping an unformatted invoice/RFP PDF or product damage photo to see OpsAgent parse and process it live on screen.
- **The 6-Week Readiness Assessment**: Offer a complimentary 1-day **"3-6-5 AI Assessment"** for regional SMEs to evaluate their current M365 licensing and data readiness.

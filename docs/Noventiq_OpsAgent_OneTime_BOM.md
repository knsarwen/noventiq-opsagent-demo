# Noventiq OpsAgent: One-Time Detailed Bill of Materials (BOM)

**Project Name**: Noventiq OpsAgent Demo & PoC Hub (UOB Summit 2026)  
**Cost Model**: **One-Time Implementation & Demo Build** (Not Monthly Recurring)  
**Architecture Principle**: **100% Low-Code / No Custom Azure Functions Needed**

---

## 1. Executive Summary & Cost Structure

The **Noventiq OpsAgent** solution is engineered strictly around native Microsoft 365, Copilot Studio, Power Platform, and minimal consumption-based Azure AI services. 

### Key Architectural Highlights:
- **Zero Custom Code Infrastructure**: **NO Azure Functions, Web Apps, App Services, or custom API microservices are required.** All business logic, orchestration, and API calls run natively inside **Copilot Studio** and **Power Automate**.
- **One-Time Project Budgeting**: All development labor, setup, and consumption required to build, test, freeze, and present the demo live at the UOB Summit are calculated as a **one-time investment**.

---

## 2. One-Time Professional Services & Implementation BOM (Labor)

Effort is calculated across **128 Total Man-Hours** (from 17 August to 28 September 2026). Standard regional professional services rates are applied for reference ($100 USD/hr blended average).

| Item # | Role / Work Component | Description & Scope | Hours | Rate (USD) | Line Total (USD) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **1.1** | **Agentic AI & Power Platform Architect** | Dataverse Schemas, Copilot Studio Agent Core, Teams Adaptive Cards (v1.5), Security & DLP config. | 48 hrs | $110 / hr | $5,280 |
| **1.2** | **Power Automate & Azure AI Engineer** | Azure AI Doc Intel setup, GPT-4o Vision API Integration, Word-to-PDF engine, Flow workflows. | 44 hrs | $100 / hr | $4,400 |
| **1.3** | **Business Transformation & Pitch Lead** | Storyboarding, 6-Slide Presentation Deck, Booth Collateral & Executive Presentation Rehearsals. | 24 hrs | $110 / hr | $2,640 |
| **1.4** | **QA & Demo Coordinator** | End-to-end scenario testing, latency tuning, and 4K backup screen recording. | 12 hrs | $70 / hr | $840 |
| **SUBTOTAL** | **PROFESSIONAL SERVICES LABOR** | **One-Time Implementation Effort** | **128 hrs** | **Blended** | **$13,160 USD** |

---

## 3. One-Time Azure & M365 Consumption BOM (Demo & Event Build)

For the demonstration build, testing (approx. 250 test executions), and live Summit presentation day, Azure AI and M365 services operate on pay-as-you-go consumption. *(These costs are typically covered under standard Microsoft Partner Azure Credits / Sandbox Subscriptions).*

| Item # | Technical Component | SKU / Meter | Consumption Estimate for Demo Build & Event | One-Time Cost (USD) |
| :--- | :--- | :--- | :--- | :--- |
| **2.1** | **Azure AI Document Intelligence** | Layout & Prebuilt Invoice/PO Model | ~300 pages analyzed (testing + live demo) @ $0.01 / page | $3.00 |
| **2.2** | **Azure OpenAI Service (GPT-4o Vision)** | `gpt-4o` Vision Model Endpoint | ~200 defect image calls (~500k input/output tokens) | $8.50 |
| **2.3** | **Microsoft Copilot Studio** | Messages / Action Plugins | ~500 test & demo session turns (within M365 trial/partner credit) | $0.00 *(Partner Credit)* |
| **2.4** | **Power Automate & Dataverse** | Power Automate Per Flow / Dataverse Storage | Sandbox / Developer Environment allocation | $0.00 *(Partner Credit)* |
| **2.5** | **Custom Azure Code (Azure Functions / Web Apps)** | **NOT REQUIRED** | **$0.00 (Zero custom code required)** | **$0.00** |
| **SUBTOTAL** | **AZURE & M365 CONSUMPTION** | **Demo Build & Event Execution** | **Pay-as-you-go Sandbox** | **~$11.50 USD** |

---

## 4. Technical Architecture Bill of Materials (Software & Components)

```
+-----------------------------------------------------------------------------------+
|                        NOVENTIQ OPSAGENT TECHNICAL BOM                             |
+-------------------+-------------------+-------------------+-------------------+---|
| COMPONENT         | SERVICE / TOOL    | LICENSING TYPE    | CUSTOM CODE NEEDED|
+-------------------+-------------------+-------------------+-------------------+---|
| Agent Orchestration| Copilot Studio    | Low-Code Platform | NONE (Native)     |
| Document Extraction| Azure AI Doc Intel| Azure Consumption | NONE (Prebuilt)   |
| Vision Triage     | Azure OpenAI      | Azure Consumption | NONE (Prompt Only)|
| Data & Storage    | Dataverse         | Power Platform    | NONE (Dataverse)  |
| Workflow Engine   | Power Automate    | M365 / Power Auto | NONE (Low-Code)   |
| Interactive UI    | Teams Adaptive Card| Native Teams v1.5 | NONE (JSON Schema)|
| Customer Dispatch | Outlook Connector | Native M365       | NONE (Native)     |
+-------------------+-------------------+-------------------+-------------------+------------------+
```

---

## 5. Master One-Time Investment Summary

```
====================================================================================
               NOVENTIQ OPSAGENT DEMO & POC HUB - ONE-TIME BOM SUMMARY              
====================================================================================
 1. Professional Services & Engineering (128 Man-Hours) --------->  $13,160.00 USD
 2. Azure AI & Cloud Sandbox Consumption --------------------------->       $11.50 USD
 3. Infrastructure & Custom Code (Azure Functions) ----------------->        $0.00 USD
====================================================================================
 TOTAL ONE-TIME INVESTMENT ESTIMATE ------------------------------->  $13,171.50 USD
====================================================================================
```

### Key Customer Takeaway for the Summit:
By eliminating custom code infrastructure (like Azure Functions or custom Web Apps), Noventiq saves the SME **tens of thousands of dollars in ongoing cloud maintenance, DevOps overhead, and custom code refactoring.**

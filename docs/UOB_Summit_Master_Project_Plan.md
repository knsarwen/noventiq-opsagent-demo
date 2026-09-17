# Master Project Plan & Timeline: Noventiq OpsAgent UOB Summit

## 📅 Executive Timeline Overview

- **Start Date**: Monday, 17 August 2026  
- **Internal Freeze Date (1 Week Prior)**: Monday, 21 September 2026  
- **Event Date**: Monday, 28 September 2026  
- **Total Working Window**: 6 Weeks (5 Weeks Active Build + 1 Week Dry Run/Buffer)

---

## 🗓️ Phase-by-Phase Timeline Breakdown

```mermaid
gantt
    title Noventiq OpsAgent UOB Summit Master Roadmap (17 Aug - 28 Sept 2026)
    dateFormat  YYYY-MM-DD
    section Phase 1: Planning
    Research & Discovery          :p1a, 2026-08-17, 2026-08-21
    Azure & M365 Setup            :p1b, 2026-08-19, 2026-08-23
    section Phase 2: PoC Hub Build
    Dataverse / Fabric Schemas    :p2a, 2026-08-24, 2026-08-28
    AI Intelligence Provisioning  :p2b, 2026-08-26, 2026-08-30
    section Phase 3: Demo Development
    Process 1 (Quote Engine)      :p3a, 2026-08-31, 2026-09-06
    Process 2 (Warranty Vision)   :p3b, 2026-09-04, 2026-09-11
    Copilot Studio Agent Core     :p3c, 2026-09-07, 2026-09-13
    section Phase 4: Pitch & Polish
    Slide Deck & Storyboard       :p4a, 2026-09-14, 2026-09-18
    End-to-End Live Testing       :p4b, 2026-09-16, 2026-09-20
    section Phase 5: Freeze & Buffer
    Internal Freeze & Dry Run     :crit, p5a, 2026-09-21, 2026-09-25
    Backup Video Recording        :p5b, 2026-09-22, 2026-09-26
    Summit Presentation Day       :milestone, m1, 2026-09-28, 1d
```

---

## 📑 Detailed Work Breakdown Structure (WBS)

### Phase 1: Research, Architecture & Azure Environment Provisioning
**Dates**: 17 Aug – 23 Aug 2026 (Week 1)
- **Research & Requirements Alignment**:
  - Finalize sample document schemas (B2B RFP PDF, Purchase Orders, Tax Invoice Receipt).
  - Finalize equipment defect photos for GPT-4o Vision triage demonstration.
- **Azure & Power Platform Tenant Setup**:
  - Provision Azure AI Document Intelligence service instance.
  - Provision Azure OpenAI Service instance (Deploy `gpt-4o` vision model endpoint).
  - Configure Power Platform environment (Dataverse, Copilot Studio, Power Automate DLP rules).

---

### Phase 2: PoC Hub & Data Infrastructure Setup
**Dates**: 24 Aug – 30 Aug 2026 (Week 2)
- **Dataverse & Fabric OneLake Setup**:
  - Create Customer Master & Credit Ledger tables in Dataverse.
  - Create Product Catalog, MOQs, & Stock Inventory master tables.
- **AI Intelligence & Document Processing**:
  - Test Azure AI Document Intelligence zero-template extraction against sample RFPs.
  - Build Power Automate custom HTTP action for Azure OpenAI GPT-4o Vision API.

---

### Phase 3: Core Demo & PoC Development
**Dates**: 31 Aug – 13 Sept 2026 (Weeks 3 & 4)
- **Process 1 Build (B2B Quote Approval)**:
  - Build Power Automate flow for RFP ingestion $\rightarrow$ Dataverse credit check $\rightarrow$ ERP inventory check.
  - Design Word Quote Template (`.docx`) & PDF conversion flow.
  - Build Teams Adaptive Card (v1.5) for 1-click management approval.
- **Process 2 Build (Warranty Claim & Technical Triage)**:
  - Build Power Automate flow for Warranty Claim receipt processing.
  - Build GPT-4o Vision diagnostic triage flow & validity scoring.
  - Build stock reservation logic & Finance Credit Note approval Adaptive Card.
- **Copilot Studio Agent Core**:
  - Orchestrate all flows into **Copilot Studio Agent Core** (Action plugins, topic triggers, generative answers).

---

### Phase 4: Pitch Preparation, Deck & End-to-End Integration
**Dates**: 14 Sept – 20 Sept 2026 (Week 5)
- **Pitch Deck Development**:
  - Draft Slide Deck following the **3-6-5 Playbook** structure (6 Slides).
  - Finalize ROI metrics, SME value propositions, and Noventiq booth conversion strategy.
- **Integration & Demo Rehearsal**:
  - Conduct full end-to-end dry run of Process 1 & Process 2.
  - Refine prompt responses and execution speed.

---

### Phase 5: Internal Freeze, Buffer Week & Summit Execution
**Dates**: 21 Sept – 28 Sept 2026 (Week 6 - **Freeze Week**)
- **Target Deadline**: **21 September 2026 (Feature Freeze)**
- **Activities**:
  - Record 4K backup execution video of both demo flows (failsafe against venue Wi-Fi drops).
  - Executive dry-run & rehearsal with Raymond Chow / Jessica Tan.
  - **28 September 2026**: **UOB Summit Live Presentation & Booth Showcase**.

---

## 🎯 Summary Milestones & Deliverables

| Date | Milestone | Key Deliverable |
| :--- | :--- | :--- |
| **23 Aug 2026** | **M1: Foundation Ready** | Azure AI & Power Platform environment fully provisioned. |
| **30 Aug 2026** | **M2: Data & AI Hub Ready** | Dataverse mock tables & GPT-4o Vision API working. |
| **13 Sept 2026** | **M3: Demo Build Complete** | Process 1 & Process 2 functional in Copilot Studio. |
| **20 Sept 2026** | **M4: Pitch & Integration Complete** | Deck finalized & end-to-end integration tested. |
| **21 Sept 2026** | **M5: INTERNAL FREEZE** | Code frozen, backup recordings complete, rehearsals ongoing. |
| **28 Sept 2026** | **M6: UOB SUMMIT EVENT** | Live presentation & booth demo execution. |

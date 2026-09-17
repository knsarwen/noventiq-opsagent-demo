# Noventiq OpsAgent: Hotel Domain Facilities & Event Booking Demo Blueprint

**Project Theme**: The Pragmatic 3-6-5 AI Playbook for Capital-Efficient AI Capabilities  
**Use Case**: Hotel & Hospitality Facilities Booking (Boardroom, Event Hall & Catering Inquiry-to-Quotation)  
**Architecture Principle**: 100% Low-Code / Microsoft 365 + Copilot Studio + Power Platform  

---

## 🏨 1. Hotel Domain Workflow Overview: Inquiry-to-Quotation

In the hospitality sector, corporate clients, event planners, and guests frequently send unstructured email inquiries for **Boardroom bookings, Grand Ballroom galas, corporate seminars, or catering packages**. 

Currently, sales & event management teams spend hours manually checking calendar availability, calculating equipment/catering pricing, getting manager sign-off on discounts, and drafting quotation proposals. **Noventiq OpsAgent** automates this end-to-end in **under 30 seconds**.

```
+---------------------------------------------------------------------------------------------------+
|                        HOTEL FACILITIES INQUIRY-TO-QUOTATION WORKFLOW                              |
+---------------------------------------------------------------------------------------------------+
| 1. INGESTION     | 2. EXTRACT        | 3. AVAILABILITY   | 4. DRAFT QUOTE   | 5. GOVERN        | 6. DISPATCH |
| Guest Inquiry    | AI Parser         | Calendar & Rates  | PDF Generator    | Manager Approval | Sales Email |
| Email / RFP      | Room, Pax, Dates  | Dataverse / Outlook| Word Template    | Teams Card       | Outlook     |
+---------------------------------------------------------------------------------------------------+
```

---

## 🛠️ 2. Step-by-Step Technical & Functional Feasibility

| Step # | Action Item | Department Aligned | How OpsAgent Works (Technical Mechanics) | Microsoft Tech Stack Used | Technical Feasibility |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **1** | **Receive Inquiry Email** | Events / BD / Front Desk | OpsAgent monitors shared mailboxes (e.g. `events@hotel.com`) via Power Automate trigger when a new inquiry or RFP arrives. | **Office 365 Outlook Connector** + **Power Automate** | 🟢 100% Ready (Native Trigger) |
| **2** | **Extract Inquiry Requirements** | Sales & Reservations | Extracts event date, room type (e.g. Executive Boardroom, Grand Ballroom), number of guests (pax), seating style (U-shape/Banquet), and add-ons (AV/Catering) from unstructured body text or attached RFP/PDF. | **Copilot Studio** + **Azure AI Document Intelligence** / **AI Builder** | 🟢 100% Ready (Prebuilt Parser) |
| **3** | **Check Availability & Calculate Rates** | Operations / Revenue Management | Automatically queries room reservation schedule and rate card master table to check if the facility is open on requested dates & calculates baseline venue + catering package pricing. | **Power Automate** + **Dataverse** (or **Outlook Shared Resource Calendar** / **SharePoint List**) | 🟢 100% Ready (Low-Code Query) |
| **4** | **Draft Branded Quotation Proposal** | Sales Operations / Commercial | Populates a professional Hotel Event Proposal document with customer details, room layout, itemized breakdown (room fee, AV setup, coffee break catering), and deposit terms. Converts automatically to PDF. | **Power Automate (Populate Word Template to PDF)** | 🟢 100% Ready (Native Word/PDF Engine) |
| **5** | **Management / Revenue Approval** | Finance / Revenue Director | If a custom discount is requested or peak date booking is flagged, OpsAgent sends an interactive Teams Adaptive Card to the Sales/Revenue Director with a 1-click **Approve / Reject / Adjust** button. | **Teams Adaptive Cards (v1.5)** + **Power Automate Approvals** | 🟢 100% Ready (Native Teams Card) |
| **6** | **Dispatch Quote to Sales Personnel** | Sales Representative | Once approved, OpsAgent creates a pre-formatted draft email in Outlook attached with the official PDF quotation. The sales manager reviews and clicks **Send**. | **Outlook Connector (Create Draft Email)** | 🟢 100% Ready (Native Draft Action) |

---

## 📐 3. Mapping to "The 5 Universal AI Capabilities" (Slide 3 Alignment)

This hotel booking use case perfectly maps to the **5 Universal Capabilities** featured in the presentation deck:

1. **UNDERSTAND (Ingestion & Extraction)**: OpsAgent reads unstructured emails and PDF RFPs for boardroom specs, attendee count, catering requests, and dates.
2. **CONNECT (Live System Query)**: OpsAgent queries the hotel facility calendar and room rate matrix in Dataverse/SharePoint without sales needing to call front-desk operations.
3. **GENERATE (Quotation & Proposal)**: OpsAgent dynamically generates a customized, branded PDF event quotation with itemized venue and meal rates.
4. **GOVERN (Approval & Compliance)**: OpsAgent posts an interactive Teams Adaptive Card to the Revenue Director to approve custom packages or non-standard discounts.
5. **EXECUTE (Action & Communication)**: OpsAgent prepares the finalized email draft in the Sales Manager's Outlook inbox ready for one-click customer dispatch.

---

## 🎯 4. Demo Execution Script & Sample Scenario (For Summit Presentation)

### Demo Scenario: "Grand Executive Boardroom & Corporate Seminar Booking"

* **Customer Email Received**:  
  > *"Hi Events Team, We would like to book the Executive Boardroom for 25 pax on 15th October 2026 for a full-day strategy session. Please include morning tea, lunch buffet, and high-speed AV setup. Can you offer a 10% corporate package discount? Thanks, Sarah (TechCorp SG)."*

* **Live 30-Second Automation Execution**:
  1. **00:03s**: Power Automate detects email in `events@hotel.com`.
  2. **00:08s**: Copilot Studio parses parameters: `Room: Executive Boardroom`, `Pax: 25`, `Date: 15-Oct-2026`, `Package: Full-Day + Catering + AV`, `Discount Requested: 10%`.
  3. **00:14s**: Dataverse query verifies: *Boardroom is AVAILABLE on 15-Oct-2026*. Baseline total = $2,500 SGD. Discounted total = $2,250 SGD.
  4. **00:20s**: Adaptive Card arrives in Teams `#Events-Approvals` channel. Revenue Manager clicks **"Approve Discount"**.
  5. **00:27s**: Branded `TechCorp_Boardroom_Quotation.pdf` is created and attached to an Outlook draft email addressed to Sarah.
  6. **00:30s**: Sales Manager clicks **Send**.

---

## 🚀 5. Summary Verdict for Management Review

- **Technical Feasibility**: **100% FEASIBLE out of the box**.
- **Setup Time**: **2 to 3 Days** for full demo build & freeze.
- **Cost**: **$0.00 Custom Code / Infrastructure**. Uses standard M365 & Power Platform capabilities already owned by SMEs.

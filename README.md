# 📊 Automation, Workflow & Serverless Visualization Portfolio
**Edson Quinas | Cloud Operations Engineer**

Welcome to my operations portfolio. This repository contains hands-on projects demonstrating how I solve complex business problems through automated workflows, custom serverless visualization tools, and zero-cost infrastructure data engineering.

---

## 🚨 Project 1: Dynamic Data Routing & Exception Handling

* **Overview:** Cross-reference mismatched service order dates against master regional datasets.

* * **Tools Used:** Power Automate, Office 365 Outlook / Excel  

* **Key Feature:**
  - Dynamic cross-referencing between multiple datasets
  - Proactive error prevention and exception routing
  - Real-time string manipulation for targeted data matching
* 📁 **[View Project Details & Proof](./dynamic-data-routing-and-exception-handling/)**

---

## 📊 Project 2: ETA Mismatch "Smart Merge" Deduplication Engine

**Overview:** Engineered a custom data reconciliation dashboard to catch SLA discrepancies between Proposed Dates and ETA dates.
**Tools Used:** JavaScript (Map Objects), PapaParse, Chart.js
**Key Features:**
*   **Asynchronous Reconciliation:** Custom "Smart Merge" algorithm utilizing JS Maps to dynamically reduplicate records and update historical ticket statuses in real-time.
*   **Error-Proof Data Parsing:** Strict `try...catch` ingestion loops to safely bypass corrupted text strings and malformed dates without crashing the UI.
*   **Actionable KPI Generation:** Live percentage calculators for timeout ratios and daily average mismatch alerts.
* 📁 **[View Project Details & Proof](./month-end-reporting)**

---

## 📊 Project 3: Engineering Visits - Serverless Visualization Dashboard

**Overview:** Architected a "zero-compute-cost" operational dashboard to visualize live engineering SLA volumes, geographical ticket distributions, and Tech Courier dependencies. Built purely on the client-side to eliminate backend hosting and database costs.

* **Tools Used:** Power BI (Web), Excel, JavaScript (ES6+), D3.js, Chart.js, HTML5/CSS, LocalForage (IndexedDB), TopoJSON
* **Key Features:**
  - Total request tracking (KPI)
  - Zero-Cost Architecture: Ingests raw CSV exports entirely in the browser memory using IndexedDB, bypassing standard local storage limits.
  - Ticket volume trends over time
  - Geographical Density Mapping: Interactive UK topology map rendering scalable volume nodes.
* 📁 **[View Project Details & Proof](./engineering-visits-serverless-visualization-dashboard)**

---

## ⚙️ Project 4: Finance Approval Workflow Automation

**Overview:** Built an automated finance approval workflow using Power Automate that routes requests based on thresholds, sends notifications, and logs outcomes to ensure consistent and auditable decision-making.

* **Tools Used:** Power Automate  
* **Key Features:**
  - Threshold-based approval logic
  - Automated and manual approval routing
  - Email notifications for approval outcomes
  - Structured logging for auditability
* 📁 **[View Project Details & Proof](./finance-approval-workflow)**

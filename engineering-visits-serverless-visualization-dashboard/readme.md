⚙️ Project: Engineering Visits Serverless Visualization Dashboard


## 🎯 Objective
Design and engineer a "zero-compute-cost" operational dashboard to visualize live engineering SLA volumes, geographical ticket distributions, and Tech Courier dependencies. The solution required a purely client-side architecture to process large datasets without incurring backend hosting or database infrastructure costs.

---

### 🧩 Dashboard Overview
(Note: Sensitive PII, Request IDs, and specific problem codes have been redacted to ensure strict BPSS compliance.)
![Overview](overview.png)

---

### 🛠️ Architecture & Execution

• Engineered a resilient client-side data ingestion and storage pipeline:
  - Utilised PapaParse to natively parse raw CSV exports directly within the browser
  - Implemented IndexedDB (via LocalForage) to bypass strict 5MB browser quotas and handle massive datasets asynchronously
  - Built strict try...catch loops to safely intercept corrupted strings and malformed dates without crashing the UI

• Developed a custom "Smart Merge" deduplication algorithm:
  - Leveraged JavaScript Map objects to actively reconcile ticket lifecycles and prevent reporting duplication
  - Dynamically isolated and matched standard Request IDs across multiple CSV uploads
  - Generated fallback "ghost IDs" (combining Date, Engineer, and Site) to safely process legacy rows missing primary keys

• Built modular, theme-responsive visualisations to map operational data:
  - Engineered an interactive UK geographical density map using D3.js and TopoJSON (d3.geoMercator()) to dynamically render SVG volume nodes based on coordinates
  - Deployed Chart.js to map Area Profiles (Doughnut), Engineer Load (Stacked Bars), and Contextual Trend Lines

• Designed a dynamic front-end filtering system:
  - Integrated Flatpickr to scan the aggregated dataset and automatically disable dates with no available data
  - Locked navigation to ensure users can only query valid, active operational windows

---

## 📸 Proof of Execution

### ✅ KPI Metrics & Volume Tracking
![data](data.png)
Interactive KPI cards displaying Total Volume, Top 10 Engineer %, Average Daily Calls, and Top 10 Sites %.
Designed with CSS hover transitions for dynamic UI response.

---
 
### ✅ Geographical Density & Area Profiling
![data2](data2.png)
D3.js UK topology map with custom hover states raising specific volume nodes to the front of the Z-index. 
Rendered alongside Top 10 Address bar charts and Area Doughnut charts.

---

### ✅ Volume Trend vs. Tech Courier Analysis
![data3](data3.png)
Contextual line chart isolating internal Engineering Volume against external Tech Courier usage. 
Includes Top 10 Engineers profiling (engineer names actively redacted for security compliance).

---

### ✅ Dynamic Date Filtering
![calendar](calendar.png)

Flatpickr implementation mapping specifically to ingested dataset dates, automatically restricting selection to valid operational days.

---

### ✅ Complete Call Volume Registry
![data4](data4.png)
Paginated, live-searchable registry table. Automatically excludes Tech Courier metrics to preserve internal engineering math accuracy (PII and internal Request IDs redacted).

---

## 📊 Business Impact
 • Zero Infrastructure Cost: Delivers enterprise-grade reporting and data visualization with a $0 cloud footprint.
 • Preventative Data Accuracy: The Smart Merge deduplication algorithm eliminates legacy double-counting errors natively.
 • Operational Visibility: Instantly highlights internal engineering workload spikes versus the reliance on external Tech Couriers.
 • Rapid Deployment: Can be executed instantly in any modern browser without requiring database spin-ups, API configurations, or software installations.

---

### ✅ Key Takeaways
• Demonstrated advanced ability to utilize browser-native storage (IndexedDB) for complex data engineering.
• Applied advanced data structures (Maps, Sets) to process, clean, and reconcile unformatted reporting data.
• Engineered complex D3.js and Chart.js DOM manipulations tied to a unified, responsive CSS variable theme structure.
• Displayed strict adherence to data security standards by architecting local-only execution and maintaining BPSS compliance guidelines.

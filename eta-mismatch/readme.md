⚙️ Project: ETA Mismatch Tracker

--- 
## 🎯 Objective
To identify, monitor, and resolve discrepancies between forecasted Estimated Times of Arrival (ETA) and actual system timestamps. This solution provides immediate visibility into timing variances, ensuring stakeholder alignment and preventing cascading delays in downstream operations.

---
## 🧩 Dashboard Overview 
A lightweight, responsive HTML-based interface designed for quick diagnostic views. The dashboard highlights critical ETA mismatches using visual indicators (e.g., color-coded variance thresholds) and allows users to filter discrepancies by severity, date, or specific categories. It transforms raw timestamp data into an easily readable format for operational review.

---
## ⚒️ Arquitecture and Execution

• Frontend Interface: 
  - Built utilizing HTML, CSS, and lightweight JavaScript to ensure a fast, responsive user experience without heavy framework dependencies.

• Data Ingestion: 
  - Automatically parses and standardizes incoming timestamp data to compare expected ETAs against actual logged times.

• Logic & Processing:
  - Implements conditional formatting rules to calculate the time delta. Mismatches exceeding the acceptable tolerance threshold are flagged and pushed to the forefront of the dashboard.

• Deployment: 
  - Packaged as a standalone portfolio asset, demonstrating front-end structuring and data visualization principles.

---
## 📷 Proof of Execution
(Insert Picture 1: Wide shot of the main HTML dashboard interface showing the overall layout)
(Insert Picture 2: Close-up of a flagged ETA mismatch with conditional formatting)
(Insert Picture 3: View of the filtering or sorting mechanism in action)
(Insert Picture 4: Code snippet showcasing the logic used to calculate the time delta)
(Insert Picture 5 - Optional: View of the mobile/responsive scaling of the dashboard)

---
## 📊 Business Impact
Operational Visibility: Eliminated blind spots regarding timing discrepancies, allowing teams to proactively address delays rather than reacting to them post-failure.
Process Efficiency: Replaced manual timestamp cross-referencing with an automated, at-a-glance dashboard, saving significant administrative time per week.
Data Accuracy: Improved the integrity of reporting by establishing a single source of truth for tracking expected versus actual performance metrics.

---


### ✅ Key Takeaways
• Demonstrated advanced ability to utilize browser-native storage (IndexedDB) for complex data engineering.
• Applied advanced data structures (Maps, Sets) to process, clean, and reconcile unformatted reporting data.
• Engineered complex D3.js and Chart.js DOM manipulations tied to a unified, responsive CSS variable theme structure.
• Displayed strict adherence to data security standards by architecting local-only execution and maintaining BPSS compliance guidelines.

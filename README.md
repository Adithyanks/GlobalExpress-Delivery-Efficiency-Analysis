# Strategic Logistics Audit: GlobalExpress Delivery Efficiency

## 📌 Executive Summary
This project is a comprehensive operational audit of **GlobalExpress Logistics**, analyzing 45,000+ multi-dimensional delivery records. The goal was to move beyond surface-level reporting and identify the systemic root causes of delivery latency. By integrating transactional, driver, warehouse, and zonal datasets, I identified high-impact variables—specifically **Parking Difficulty** and **Temporal Bottlenecks**—that directly influence customer satisfaction and operational ROI.

## 🎯 The Business Challenge (COO Directives)
* **Performance Drivers:** Determine why certain deliveries exceed promised windows.
* **Environmental Impact:** Isolate the variance caused by weather/traffic vs. operational inefficiencies.
* **Geospatial Underperformance:** Identify specific "High-Risk" zones requiring intervention.

## 🛠 Technical Workflow & Data Engineering
* **Data Integrity Audit:** Cleaned and standardized 4 relational CSV datasets, handling 45,000+ rows of UUID-tagged data.
* **Advanced Feature Engineering:** Engineered a refined `Net_Delay` metric to isolate positive latencies, and derived temporal features (Weekday/Month) for trend analysis.
* **Geospatial & Demographic Clustering:** Correlated urban density and parking difficulty indices with delivery throughput.

## 💡 Strategic Insights (The "Truth" in the Data)
* **The "Parking Paradox":** My analysis revealed that **Parking Difficulty is a primary operational bottleneck**, nearly doubling delivery times—a factor more significant than vehicle type or driver bonus eligibility.
* **Temporal Volatility:** Identified a specific "Mid-Week Surge." Mondays and Wednesdays represent peak latency periods, while Tuesdays demonstrate maximum operational efficiency.
* **Zonal Risk Assessment:** Isolated **Zone 7** as a consistent outlier for underperformance, likely due to mid-range distance inefficiencies and low-density transit gaps.
* **Counter-Intuitive Findings:** Discovered that automated sorting and driver bonus schemes had negligible impacts on latency, suggesting that the bottleneck is **external (Zonal)** rather than **internal (Warehouse).**

## 🚀 Recommended Action Plan
1. **Dynamic Shift Allocation:** Increase driver capacity by 15-20% on Mondays/Wednesdays to counter systemic mid-week surges.
2. **Micro-Hub Strategy for Zone 7:** Investigate the transition to a localized "Micro-Hub" model in underperforming zones to bridge the mid-range distance gap.
3. **Parking-Optimized Routing:** Prioritize motorcycle/bicycle fleets for high "Parking Difficulty" zones to mitigate the doubling of delivery times observed in larger vehicles.

---
*Developed as part of an Advanced Data Analytics Track, focusing on actionable logistics intelligence.*

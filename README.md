# Global Logistics Optimization: Reducing Delivery Latency

## 📌 Executive Summary
This project provides a deep-dive analysis of **50,000+ logistics records** for GlobalExpress. By identifying systemic bottlenecks in the "Last-Mile" delivery phase, I developed actionable insights to improve on-time delivery rates and optimize operational costs.

## 🎯 The Business Challenge
GlobalExpress faced increasing customer churn due to unpredictable delivery windows. The objective of this analysis was to:
* **Identify geographical clusters** with the highest delay frequency.
* **Determine the correlation** between "Shipment Mode" and "Customer Rating."
* **Provide data-backed recommendations** to reduce "Late Delivery" status across high-value segments.

## 🛠 Tech Stack & Analytical Process
* **Data Orchestration:** Python (Pandas, NumPy) for cleaning inconsistent regional timestamps and handling missing values.
* **Exploratory Data Analysis (EDA):** Leveraged Seaborn and Matplotlib to visualize delivery latency and carrier performance tiers.
* **Feature Engineering:** Created "Delivery Gap" metrics to quantify the variance between estimated and actual arrival times.

## 💡 Critical Business Insights (The ROI)
* **The "Last-Mile" Bottleneck:** 42% of delays were concentrated in specific regional hubs, suggesting a requirement for localized warehouse redistribution.
* **Mode Inefficiency:** "Standard Shipping" showed a non-linear delay pattern on weekends, contributing to increased operational costs and customer support tickets.
* **Predictive Indicator:** Identified that "Product Importance" was poorly correlated with "Shipping Speed," leading to high-value customer dissatisfaction during peak periods.

## 🚀 Strategic Recommendations
1. **Dynamic Routing:** Implement a prioritized dispatch system for "High Importance" items during peak weekend windows to protect LTV (Lifetime Value).
2. **Hub Consolidation:** Re-evaluate carrier contracts in high-delay zones to target a **12% reduction in annual logistics overhead.**

---
**Note:** This project was developed as part of a specialized Data Analytics track to demonstrate the application of Python in solving complex supply-chain challenges.

# GlobalExpress – Delivery Efficiency Analysis

This repository contains a data analytics project analyzing delivery efficiency for GlobalExpress Logistics.  
The goal is to understand factors affecting delivery performance and provide actionable recommendations to improve operations.

---

## Project Overview

GlobalExpress operates multiple warehouses and delivery zones.  
The company collects data on deliveries, drivers, warehouses, and zones but has not yet fully leveraged it for operational optimization.  

This project performs **end-to-end analysis**, including data cleaning, exploratory data analysis, feature engineering, and insight generation.

---

## Dataset Description

The analysis uses the following datasets:

1. **data_deliveries.csv** – transactional data on 45,000+ deliveries including package details, delivery times, customer ratings, and costs.  
2. **data_drivers.csv** – driver information, including experience, vehicle type, ratings, and work details.  
3. **data_warehouses.csv** – warehouse details including capacity, location, refrigeration, and automation.  
4. **data_zones.csv** – delivery zone characteristics including distance, population, income, urban density, parking difficulty, and growth rate.

> All datasets are stored in the `data/` folder.

---

## Project Structure

GlobalExpress-Analysis/
│
├── data/ # CSV datasets
├── notebooks/ # Jupyter notebooks with analysis
├── requirements.txt # Python dependencies
└── README.md # Project documentation


---

## Analysis Workflow

1. **Data Loading & Cleaning**
   - Imported datasets into Pandas DataFrames.
   - Checked for missing values, duplicates, and data type consistency.
   - Handled missing values and cleaned relevant columns.

2. **Exploratory Data Analysis (EDA)**
   - Analyzed delivery times, delays, and correlations with package, driver, and zone characteristics.
   - Investigated temporal patterns (day of week, month) and operational factors (warehouse, driver, vehicle type).
   - Examined geographic and demographic patterns (distance, urban density, parking difficulty).

3. **Feature Engineering**
   - Created refined metrics, such as `delivery_time` focusing on positive delays.
   - Derived additional features for improved insight (e.g., weekday, zone grouping).

---

## Key Findings

1. **Delay Time Distribution**  
   - Delivery delays include both positive (late) and negative (early) values.  
   - A refined metric `delivery_time` focuses on positive delays.

2. **Weather & Traffic Conditions**  
   - Severe weather (stormy/snowy) and traffic conditions increase delays, but are **not the sole drivers** of performance.

3. **Temporal Patterns**  
   - Mondays and Wednesdays show higher delays; Tuesdays consistently show the lowest.

4. **Geographical & Demographic Factors**  
   - Mid-range distances have the highest delays.  
   - Low-density areas show longer delays due to travel between delivery points.  
   - Parking difficulty almost doubles delivery times and is a critical operational factor.  
   - Certain zones (e.g., Zone 7) may consistently underperform.

5. **Vehicle Type, Cost, and Profitability**  
   - No strong standalone patterns; vehicle type is not a major driver of performance.  

---

## Overall Insights

Operational and geographic factors such as **weekday scheduling, zone characteristics, density, and parking difficulty** influence delivery performance more than weather, traffic, or vehicle type.  

Additional domain-informed observations:  
- Automated sorting in warehouses did not show measurable impact in this dataset.  
- Bonus schemes did not significantly affect delivery delays.

---

## Recommendations

- **Peak Weekdays**: Increase delivery associates or add extra shifts on Mondays and Wednesdays.  
- **Tuesday Utilization**: Consider redistributing workload to optimize performance.  
- **Geographical Risks**: Prioritize underperforming zones (e.g., Zone 7) for operational improvements.  
- **Mid-Range Hubs & Parking**: Investigate routing inefficiencies and parking challenges to reduce delays.

---

## Tools & Libraries Used

- Python  
- Pandas & NumPy (data manipulation)  
- Matplotlib & Seaborn (visualizations)  
- Jupyter Notebook (analysis workflow)

---


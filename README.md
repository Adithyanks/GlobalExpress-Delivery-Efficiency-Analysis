# GlobalExpress – Delivery Efficiency Analysis

This repository presents an **end-to-end data analytics project** focused on analyzing delivery efficiency for **GlobalExpress Logistics**.  
The objective is to identify operational, temporal, and geographical factors affecting delivery performance and translate insights into actionable recommendations.

This project emphasizes **exploratory data analysis, structured reasoning, and business-oriented insights**, rather than predictive modeling.

---

## Project Objective

GlobalExpress operates across multiple warehouses and delivery zones, collecting large volumes of operational data.  
However, this data has not been fully leveraged to understand **why delivery delays occur** and **which factors matter most**.

This analysis aims to:
- Explore delivery delay patterns
- Identify operational bottlenecks
- Understand geographic and temporal risk factors
- Provide data-backed recommendations for efficiency improvement

---

## Dataset Overview

The analysis uses four structured datasets:

- **`data_deliveries.csv`**  
  Delivery-level transactional data (45,000+ records), including package details, promised vs actual delivery times, costs, customer ratings, and operational conditions.

- **`data_drivers.csv`**  
  Driver attributes such as experience, ratings, vehicle type, work preferences, and eligibility for bonuses.

- **`data_warehouses.csv`**  
  Warehouse-level information including capacity, location, automation, refrigeration, and operational costs.

- **`data_zones.csv`**  
  Delivery zone characteristics such as distance from hub, population, income, urban density, parking difficulty, and growth rate.

All datasets are available in the `data/` directory.

---

## Repository Structure
GlobalExpress-Analysis/
│
├── data/                # Raw CSV datasets
├── notebooks/           # Jupyter notebooks with full analysis
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation

---

## Analysis Workflow

### 1. Data Loading & Validation
- Loaded all datasets using Pandas.
- Verified dataset shapes, data types, duplicates, and missing values.
- Assessed data quality issues that could affect analysis.

### 2. Data Cleaning
- Handled missing numerical values where required.
- Ensured consistent data types across related datasets.
- Prepared clean, analysis-ready DataFrames.

### 3. Exploratory Data Analysis (EDA)
The EDA focused on understanding delivery delays across multiple dimensions:

- **Time-based analysis**  
  - Weekday and monthly delivery patterns  
- **Operational factors**  
  - Warehouse, driver, and vehicle attributes  
- **Geographical and demographic factors**  
  - Distance from hub, urban density, income levels  
- **External conditions**  
  - Weather and traffic conditions  

Visualization techniques (histograms, boxplots, scatterplots) were used extensively to reveal patterns.

### 4. Feature Engineering
- Created a refined delay metric (`delivery_time`) focusing only on **positive delays**.
- Derived additional features such as weekday indicators to support deeper analysis.

---

## Key Findings

### 1. Delivery Delay Distribution
- Delivery delays include both early and late deliveries.
- Focusing only on positive delays provided clearer insight into operational inefficiencies.

### 2. Weather & Traffic Conditions
- Severe weather (stormy/snowy) and heavy traffic increase delays.
- These factors contribute to delays but are **not the primary drivers** of performance issues.

### 3. Temporal Patterns
- **Mondays and Wednesdays** consistently show higher delays.
- **Tuesdays** show the lowest delays, suggesting potential for workload redistribution.

### 4. Geographic & Demographic Factors
- **Mid-range distances from hubs** experience higher delays.
- **Low-density zones** show longer delays due to increased travel time between delivery points.
- **Parking difficulty** nearly doubles delivery delays and is a critical operational constraint.
- Certain zones (e.g., **Zone 7**) consistently underperform and require focused investigation.

### 5. Vehicle Type, Cost & Profitability
- No strong standalone relationship was observed.
- Vehicle type alone is not a major driver of delivery performance.

---

## Overall Insights

Delivery performance is influenced more by **operational scheduling and geographic characteristics** than by weather, traffic, or vehicle type alone.

Key influencing factors include:
- Weekday demand patterns
- Zone-level characteristics
- Urban density
- Parking difficulty

---

## Recommendations

- **Peak Weekdays**  
  Increase delivery associates or add extra shifts on Mondays and Wednesdays.

- **Tuesday Utilization**  
  Redistribute workload from high-delay days to Tuesdays where performance is strongest.

- **Geographical Risks**  
  Prioritize underperforming zones (e.g., Zone 7) for operational audits and route optimization.

- **Routing & Parking Constraints**  
  Investigate routing inefficiencies in mid-range zones and address parking challenges to reduce delays.

---

## Tools & Technologies

- Python  
- Pandas & NumPy  
- Matplotlib & Seaborn  
- Jupyter Notebook  

---

## Notes & Limitations

- Some relationships required assumptions due to indirect links between datasets.
- Correlation analysis alone was insufficient; most insights were derived from exploratory visual analysis.
- Findings are descriptive and intended to support operational decision-making.





   

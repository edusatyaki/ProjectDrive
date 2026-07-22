# NYC Yellow Taxi 2025 - Final Report (Detailed Template)

**Group:** Group-C
**Owner:** Pallabi (Not provided)

> This is a detailed report outline, not a finished report. Work through each section below and
> replace the italicized placeholder text with your own analysis and findings.

## 1. Executive Summary
_Fill in last: 3-5 sentences summarizing the problem, your key finding, and your top recommendation._

## 2. Problem Statement

**Context:** Understanding ride demand and revenue patterns helps city planners and drivers/fleet operators optimize dispatch and working hours.

**Question this project answers:** see Section 5 below.

**Stakeholders / audience:** NYC TLC / city planners, taxi drivers and fleet operators.

## 3. Dataset Overview

**Source:** NYC Yellow Taxi 2025 trip records.

**Key fields:**
- pickup/dropoff datetime and location IDs
- passenger_count, trip_distance
- fare_amount, tip_amount, total_amount
- congestion_surcharge, airport_fee

**Size / time range:** Document which 2025 months are covered and total trip count.

**Known data quality caveats:** Watch for outlier trips (zero distance, implausibly high fares) and missing location IDs.

## 4. Methodology

### 4.1 Data Cleaning
Load the raw data, handle missing values and duplicates, fix data types, and export a clean dataset
(see the `Data Cleaning/` folder for this project).

### 4.2 Data Analysis
Explore the clean data and answer the questions in Section 5 (see `Data Analysis/`).

### 4.3 Dashboard
Turn the analysis into charts/KPIs for a non-technical audience (see `Dashboard/`).

### 4.4 Reporting
Tie cleaning, analysis, and dashboard work into the narrative in this document.

## 5. Key Analysis Questions

### 5.1 Demand Patterns
- How does ride demand vary by hour of day and day of week? When are the peak windows?

### 5.2 Fare & Tip Behavior
- What do fare and tip distributions look like, and what factors drive higher tips?

### 5.3 Airport vs Standard Trips
- How do airport trips compare to standard trips on fare, distance, and tip rate?

### 5.4 Congestion Surcharge Impact
- What is the revenue impact of the congestion surcharge on driver earnings, and how has it trended?

### 5.5 Driver Revenue Optimization
- Which time windows or zones are most profitable for drivers to work?

## 6. Results

### 6.1 Demand Patterns
_Fill in with the numbers, charts, and findings that answer the Demand Patterns questions above._

### 6.2 Fare & Tip Behavior
_Fill in with the numbers, charts, and findings that answer the Fare & Tip Behavior questions above._

### 6.3 Airport vs Standard Trips
_Fill in with the numbers, charts, and findings that answer the Airport vs Standard Trips questions above._

### 6.4 Congestion Surcharge Impact
_Fill in with the numbers, charts, and findings that answer the Congestion Surcharge Impact questions above._

### 6.5 Driver Revenue Optimization
_Fill in with the numbers, charts, and findings that answer the Driver Revenue Optimization questions above._

## 7. Recommendations
- **Immediate:** _what should change right away based on these findings?_
- **Medium-term:** _what should be monitored or tested next?_
- **Longer-term / further research:** _what would a deeper follow-up analysis add?_

## 8. Limitations & Assumptions
_List data quality issues, scope limits, and any assumptions made during cleaning or analysis._

## 9. Next Steps
_What would you do with more time or data?_

## Appendix: Progress snapshot (auto-generated)
- **Data Cleaning:** `Cleaned Dataset`, `NYC_Data_Cleaning.ipynb`, `Raw Dataset`
- **Data Analysis:** `NYC_Taxi_Data_Analysis_and_Statistics.ipynb`
- **Dashboard:** `airport_vs_standard.csv`, `congestion_surcharge.csv`, `driver_revenue.csv`, `hourly_demand.csv`, `monthly_summary.csv`, `tip_analysis.csv`

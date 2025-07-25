# Uber Fares Data Analysis using Power BI


##  1. Introduction

This project presents a data analysis of the **Uber Fares Dataset**, with the goal of uncovering patterns in ride fares, time-based trends, and operational insights. We utilized **Python (Pandas)** for data cleaning and feature engineering, and **Power BI** for data visualization and dashboard creation.

## Objective:
- Analyze fare distribution and ride characteristics  
- Discover hourly, daily, and seasonal ride patterns  
- Identify peak demand periods and pricing trends  
- Create an interactive Power BI dashboard for business use

---

## 2. Methodology

###  Data Collection:
- Source: [Kaggle – Uber Fares Dataset](https://www.kaggle.com/datasets/yasserh/uber-fares-dataset)


###  Data Cleaning in Python:
- Removed missing values and invalid entries (e.g. negative fares, unrealistic coordinates)
- Filtered passenger count to 1–6 only
- Detected and removed outliers in fare using the IQR method

###  Feature Engineering:
- Extracted `hour`, `day`, `month`, `day_of_week` from `pickup_datetime`
- Created `is_peak` column to label peak vs off-peak rides
- Calculated `distance` using the Haversine formula between pickup and drop-off locations

###  Final Datasets:
- `uber_fares_cleaned.csv` – after cleaning  
- `uber_fares_enhanced.csv` – with additional analytical features

---

##  3. Analysis Highlights

### Descriptive Stats:
- Average fare: ~$11  
- Median fare: ~$8  
- Most common passenger count: 1  
- Majority of rides are < 5 km

###  Time-Based Patterns:
- High ride volume during 5–8 PM (rush hours)
- Weekends show higher demand with slightly higher fare variability
- Most rides are on Fridays and Saturdays

###  Distance vs Fare:
- Strong positive correlation between ride distance and fare amount
- Outliers removed to ensure meaningful visualizations

---

##  4. Results

- **Peak hours** (7–10 AM, 4–7 PM) show higher fare averages
- **Friday evenings** and **Saturday nights** are high-traffic periods
- **Short-distance rides dominate**, but long rides contribute significantly to revenue
- The dashboard allows filtering by hour, day, distance, fare range, and peak time

---


##  6. Recommendations

Based on analysis, Uber could:
- Optimize **driver deployment** during peak hours and weekends
- Consider **dynamic pricing** during high-demand time blocks
- Promote **short-distance rides** in quieter hours to maintain revenue flow
- Use **location clustering** to identify high-potential premium ride zones

---


## Screenshots 

- `01_data_loading.png` – Loading CSV into Power BI

  ![images alt](https://raw.githubusercontent.com/Davypierre257/uber-fares-powerbi/a47590ce4d29e834b9589664ee3a4b2262b85018/MYSCREENSHOT/DATA%20LOAD.png)

  
- `02_data_cleaning.png` – Cleaning process
-  ![images alt](https://raw.githubusercontent.com/Davypierre257/uber-fares-powerbi/a47590ce4d29e834b9589664ee3a4b2262b85018/MYSCREENSHOT/b6.png)
-   ![images alt](https://raw.githubusercontent.com/Davypierre257/uber-fares-powerbi/a47590ce4d29e834b9589664ee3a4b2262b85018/MYSCREENSHOT/b4.png)
-    ![images alt](https://raw.githubusercontent.com/Davypierre257/uber-fares-powerbi/a47590ce4d29e834b9589664ee3a4b2262b85018/MYSCREENSHOT/b5.png)
-  
- 
-  
- 
- `04_dashboard_building.png` – Visuals being built
-  ![images alt](https://raw.githubusercontent.com/Davypierre257/uber-fares-powerbi/a47590ce4d29e834b9589664ee3a4b2262b85018/MYSCREENSHOT/PB.png)
- 
- `05_final_dashboard.png` – Final version of Power BI dashboard

--- ![images alt](https://raw.githubusercontent.com/Davypierre257/uber-fares-powerbi/a47590ce4d29e834b9589664ee3a4b2262b85018/MYSCREENSHOT/DASH.png)

---



# 📊 AtliQ Hotels – Revenue & Booking Data Analysis
## 📌 Overview

This project analyzes operational data from AtliQ Hotels, a multi-city hotel chain, to generate actionable insights on:

* Occupancy trends

* Revenue performance

* Booking platform contribution

* Customer behavior

The objective is to simulate a real-world business analytics scenario using Python.

## 🧠 Business Problem

Hotel management needs clarity on:

📍 Revenue distribution across cities

🏨 Room category performance

📊 Booking platform effectiveness

⭐ Customer satisfaction trends

* This project provides data-driven answers to these problems.

## 🗂️ Dataset

The project follows a star schema structure:

dim_date.csv

dim_hotels.csv

dim_rooms.csv

fact_aggregated_bookings.csv

fact_bookings.csv

### ⚠️ Dataset Disclaimer

* The dataset is part of a course and cannot be shared publicly.

To run locally:

1) Place files inside datasets/

2) Run the notebook

## ⚙️ Project Workflow

### 🏗️ Project Architecture
```
Raw Data (CSV Files)
        ↓
Data Loading (Pandas)
        ↓
Data Cleaning
        ↓
Data Transformation
        ↓
Exploratory Data Analysis (EDA)
        ↓
Business Insights Generation
```

### Data Loading

* Loaded multiple datasets using pd.read_csv()

* Created separate DataFrames:

1) df_date

2) df_hotels

3) df_rooms

4) df_agg_bookings

5) df_bookings

### Data Cleaning

❌ Removed invalid records (e.g., negative guest counts)

🔍 Identified overbooking scenarios (successful_bookings > capacity)

🧹 Handled missing values using median and logical checks

📅 Standardized date formats across datasets 

### Data Transformation

* Created new feature:

```
occupancy_percentage = successful_bookings / capacity
```

* Converted percentage values into readable format

* Merged datasets where required for analysis

### Data Analysis

Used:

* groupby()

* merge()

* concat()

* apply()


## 🚀 Key Metrics (KPI Summary)

💰 Total Revenue Realized: ₹ 1,708,536,599 

📈 Average Occupancy Rate: 58.5% 

🏆 Top Performing City: Mumbai → ₹ 668M+ (highest revenue)

🛏️ Best Room Category: RT4 (based on occupancy)

🌐 Top Booking Platform: others → ₹ 699M+ (highest contribution)

⭐ Average Customer Rating: 3.6/ 5


# 📊 Key Insights
### 📅 Occupancy Trends

* 📈 Higher occupancy during weekends

* Indicates leisure-driven demand

### 💰 Revenue Analysis

* Revenue concentrated in select cities

* Highlights dependency on key markets

### 🛏️ Room Category Insights

* Certain room types dominate bookings

* Opportunity for pricing optimization

### 🌐 Platform Contribution

*Few platforms drive majority revenue

* Scope for targeted partnerships

### ⭐ Customer Ratings

* Ratings vary across cities

* Indicates service consistency issues



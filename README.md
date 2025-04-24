# 🔌 Electric Vehicle Population Dataset – Exploratory Data Analysis

This project performs exploratory data analysis (EDA) on the **Electric Vehicle Population dataset** sourced from data.gov, focusing on electric vehicle trends across Washington State. The goal is to uncover insights related to vehicle types, electric range, pricing, manufacturer distribution, and geographic spread across counties.

---

## 📁 Dataset Source

- **Title**: Electric Vehicle Population Data  
- **URL**: [https://catalog.data.gov/dataset/electric-vehicle-population-data](https://catalog.data.gov/dataset/electric-vehicle-population-data)  
- **Publisher**: Washington State Department of Licensing  
- **Format**: CSV  
- **Records**: ~150,000 EVs (cleaned subset used: ~3,400 entries with complete fields)

---

## 🔍 Objectives

1. Inspect and clean the dataset
2. Analyze distribution of EV types and top manufacturers
3. Visualize electric range and pricing trends
4. Assess geographic (county-wise) distribution
5. Explore fuel eligibility programs (CAFV)
6. Analyze the relationship between price and range

---

## 🧹 Data Cleaning

- Removed rows with missing or invalid entries
- Converted appropriate columns to string or categorical types
- Used `.dropna()`, type conversion, and string normalization
- Converted `Postal Code`, `Model Year`, and `DOL Vehicle ID` to string for categorical treatment

---

## 📊 Visualizations & Insights

### 1. Distribution of EV Types
- Bar chart shows majority are **Battery Electric Vehicles (BEVs)**, followed by **Plug-in Hybrid Electric Vehicles (PHEVs)**

### 2. Top 5 Vehicle Makes
- Tesla leads the count, followed by **Kia**, **BMW**, **Volvo**, and **Mini**

### 3. Electric Range Distribution
- Histogram reveals most vehicles have a range between **60 to 250 miles**, with Tesla models on the higher end

### 4. County-wise Vehicle Counts
- **King County** has the highest number of EVs, followed by **Pierce** and **Snohomish**

### 5. MSRP vs Electric Range
- Scatter plot indicates a **positive correlation** between vehicle price and electric range

### 6. CAFV Eligibility Analysis
- Pie chart reveals that a **majority of EVs are CAFV eligible**, though a significant portion are ineligible due to low battery range

---

## 📈 Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

---

## 📌 Key Findings

- **Tesla dominates** the EV market in WA
- **Range and price are positively correlated**
- **Majority of EVs are eligible** under clean fuel programs
- **Urban counties** show significantly higher EV adoption

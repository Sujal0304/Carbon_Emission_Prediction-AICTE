# 📘 Carbon Emission Prediction System (AICTE Project)

## 🔍 Overview  
This project focuses on analyzing global environmental and economic data to **predict carbon emissions** and understand the factors influencing climate change.

The goal was not just to build a model, but to create a system that:
- Cleans and structures real-world messy data  
- Extracts meaningful insights  
- Predicts future emission trends  
- Can be extended for policy-level or industrial decision-making  

---

## 🎯 Problem Statement  
Carbon emissions are one of the biggest contributors to climate change. However, emission levels are influenced by multiple factors like:
- Energy consumption  
- GDP growth  
- Urbanization  
- Industrial activity  

The challenge is to **combine all these variables and predict CO₂ emissions accurately**.

---

## 📊 Dataset & Challenges  
- Source: Global climate + economic dataset  
- Size: ~13,500 rows, 28+ features  

### Major Issues Faced:
- Missing values (`NaN`, "..")  
- Non-numeric data types  
- Long and inconsistent feature names  
- Unstructured format (year-wise spread)

---

## 🛠️ Approach

### 1. Data Cleaning  
- Removed irrelevant columns (`SCALE`, `Decimals`, etc.)  
- Converted string values to numeric  
- Handled missing values carefully instead of blindly dropping rows  

---

### 2. Feature Engineering  
- Renamed complex variables into readable names  
  - Example: `CO2 emissions per capita` → `co2_per_cap`  
- Selected meaningful indicators:
  - Energy usage  
  - GDP  
  - Population  
  - Methane & Nitrous emissions  

---

### 3. Data Transformation  
- Converted dataset from **wide format → structured format**  
- Used pivoting and merging techniques to align:
  - Country  
  - Year  
  - Features  

---

### 4. Handling Missing Data  
- Analyzed missing values year-wise and country-wise  
- Selected optimal time range: **1991 – 2008**  
- Removed only high-missing segments instead of full dataset  

---

### 5. Model Building  
- Built regression-based models to predict:
  - Total CO₂ emissions  
  - Emissions per capita  

- Applied:
  - Data normalization  
  - Feature selection  
  - Model evaluation  

---

### 6. Prediction & Forecasting  
- Generated future emission trends  
- Created a forecast dataset for analysis  

---

### 7. Application Layer  
- Developed a Python-based app (`app.py`)  
- Allows users to:
  - Input parameters  
  - Get predicted emissions  

---

## 💡 Key Insights  
- Energy consumption and GDP strongly influence emissions  
- Urban population growth impacts emission levels  
- Developing regions show faster emission growth trends  

---

## 🚀 Project Highlights  
- Works on **real-world messy data (not pre-cleaned datasets)**  
- Focus on **data understanding + preprocessing**  
- Logical handling of missing values  
- Complete pipeline:

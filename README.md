# 🌾 Maize Yield Prediction Based on Weather – Rwanda

## 📘 Project Overview

This project aims to predict maize yield in Rwanda using historical **rainfall** and **temperature** data. The goal is to assess how climatic factors impact agricultural productivity, and to build a regression model capable of forecasting yield for decision-making in agriculture.

---

## 🧰 Tools & Technologies Used

- 🐍 **Python**: Data processing, regression modeling (Scikit-learn)
- 📊 **Power BI**: Dashboard and visual analysis
- 📁 **Datasets**: FAOSTAT + Visual Crossing Weather Data

---

## 📂 Datasets

### 1. **FAOSTAT – Maize Yield**
- Source: [FAOSTAT](https://www.fao.org/faostat/en/#data)
- Country: Rwanda
- Years: 2010–2023
- Metric: Maize Yield (hg/ha → tonnes/ha)

### 2. **VISUAL CROSSING – Weather Data**
- Source: [Visual Crossing Weather Datasets](https://www.visualcrossing.com/weather-data/)
- Monthly Temperature (°C) & Rainfall (mm/month)
- Aggregated to **annual** averages and totals

---

## 🧹 Data Cleaning

- Cleaned FAOSTAT dataset for maize yield in Rwanda
- Converted units to tonnes per hectare
- Aggregated weather data (monthly → annual)
- Merged datasets on the `Year` column
- Exported to `weather_data.csv` and `maize_yield_rwanda.csv`

---

## 🔍 Exploratory Data Analysis (Power BI)

Power BI was used to visualize trends and relationships:

- 📈 Maize Yield Over Time (Line Chart)
- 🌧️ Rainfall & Temperature Trends (Dual-Axis Chart)
- 📊 Yield vs. Rainfall (Scatter)
- 🌡️ Yield vs. Temperature (Scatter)
- 📋 Correlation Heatmap

🧭 **Slicers** added:
- Year
- Rainfall (mm/year)
- Temperature (°C)

- ![powerbi dashboard](https://github.com/nzizabenjamin/FINAL_PROJECT/blob/69314d8a2214afd2d7e874ef89a8a17accd04fe0/Screenshot%202025-08-03%20201507.png)

---

## 🤖 Model Building

Two regression models were built in Python to predict yield:

### 1. **Linear Regression**
- RMSE: 0.43
- R² Score: -0.14 ❌ (underfit)

### 2. **Random Forest Regressor**
- RMSE: 0.17
- R² Score: 0.82 ✅ (best fit)
- Chosen for final predictions

---

## 📁 File Structure


---

## 🧠 Key Insights

- Rainfall is a **strong predictor** of maize yield.
- Temperature has **limited influence** in the 18–20°C range.
- Best yields observed with rainfall between **1200–1500 mm/year**.

---

## 🚀 Next Steps

- Add 2024–2026 climate forecast data
- Expand model to cover other crops (e.g., beans, sorghum)
- Deploy dashboard as a web app or Power BI service
- Integrate alerts for yield drop risks

---

## 🙏 Acknowledgements

- [FAOSTAT](https://www.fao.org/faostat/)
- [Visual Crossing Weather Dataset](https://www.visualcrossing.com/weather-data/)

---

## 👨‍💻 Author

**[Nziza Benjamin]**  
Capstone Project – Introduction to Big Data Analytics  
Institution: [Adventist University Of Central Africa]

---

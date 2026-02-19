# 🌍 Global Temperature Anomaly Modeling & Climate Trend Prediction

## 📌 Domain
**Climate Science | Global Environmental Change | Geosciences**
🔗 **Reproducible Kaggle Implementation:**  
Full computational notebook available at: (https://www.kaggle.com/code/ayazlakho/global-temperature-anomaly-prediction) 

---

## 🔎 Overview

This project implements a fully reproducible climate data analysis and forecasting pipeline using the **Global Land Temperatures by City** dataset from Kaggle (Berkeley Earth).

It demonstrates:

- Temperature anomaly computation using climatological baseline
- Long-term warming trend quantification (°C per decade)
- Rolling mean climate smoothing
- Time-series forecasting using Machine Learning
- Scientific evaluation using MAE and RMSE

This project is research-focused and intended for academic portfolio demonstration.

---

## 📊 Dataset

**Name:** Global Land Temperatures by City  
**Source:** Berkeley Earth Surface Temperature Study  
**Platform:** Kaggle  
**Link:** https://www.kaggle.com/datasets/berkeleyearth/climate-change-earth-surface-temperature-data  

### Coverage
- **Temporal:** 1750–2013  
- **Spatial:** Global (cities worldwide)  
- **Records:** ~8 million rows  

---

## 🧠 Research Motivation

Climate change is assessed through **temperature anomalies**, not raw temperatures.  
Anomalies remove seasonal and spatial biases and allow consistent long-term comparison.

This project reproduces key climatology principles:

- Baseline normalization (1951–1980 reference period)
- Rolling smoothing for long-term signal extraction
- Warming rate estimation (°C/decade)
- Predictive modeling of anomaly trends

---

## ⚙️ Methodology

### 1️⃣ Data Processing
- Removed missing temperature values
- Converted date column to datetime
- Extracted year and month
- Aggregated city-level data into global monthly averages

### 2️⃣ Temperature Anomaly Computation
- **Baseline Period:** 1951–1980  
- **Formula:**  
  `Anomaly = Monthly Temperature − Baseline Mean`
- Generated anomaly time series (1750–2013)

### 3️⃣ Climate Trend Analysis
- 12-month rolling average smoothing
- Linear regression over time index
- Computed warming rate in °C per decade

### 4️⃣ Forecasting Problem

**Objective:**  
Predict next-month temperature anomaly using previous 6 months.

**Train/Test Split:**  
- 80% training  
- 20% testing  
- Time-aware split (no data leakage)

---

## 🤖 Models Implemented

### 🔹 Baseline Model
- Linear Regression

### 🔹 Advanced Model
- Random Forest Regressor

---

## 📈 Evaluation Metrics

- **MAE** — Mean Absolute Error  
- **RMSE** — Root Mean Squared Error  

---

## 📊 Key Results

- Clear warming acceleration post-1970
- Positive long-term warming slope
- Random Forest outperforms Linear Regression
- Recent lag months have highest predictive importance

---

## 📌 Generated Outputs

- Global anomaly time-series visualization
- 12-month smoothed climate trend plot
- Warming rate estimation (°C/decade)
- Model prediction comparison plot
- Feature importance analysis

---

## 🛠 Technical Stack

- **Language:** Python  
- **Libraries:**  
  - Pandas  
  - NumPy  
  - Matplotlib  
  - Seaborn  
  - Scikit-learn  
- **Environment:** Kaggle Notebook  

---

## 🎓 Research Significance

This project demonstrates:

- Strong understanding of climate anomaly methodology
- Ability to process large-scale environmental datasets
- Implementation of time-series ML models
- Scientific evaluation and interpretation
- Reproducible computational research workflow

---

## 🚀 Possible Extensions

- LSTM/GRU deep learning forecasting
- Continental or regional anomaly modeling
- Extreme event detection
- Structural break analysis (post-1970 acceleration)
- Multi-variable climate modeling (CO₂, precipitation, ENSO)

---

## 📌 Academic Intent

This repository is intended for research portfolio development and academic outreach.  
The focus is methodological rigor, reproducibility, and scientific understanding — not deployment.

---

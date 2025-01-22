# Greenhouse Gas Emissions Analysis and Forecasting in India 🌍

This repository provides a comprehensive analysis and forecasting of Greenhouse Gas (GHG) emissions in India. Utilizing advanced statistical models, machine learning techniques, and econometric analysis, the project aims to identify key contributors to emissions, analyze volatility, and create predictions for future trends.

---

## 📋 Table of Contents

1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
4. [Models Implemented](#models-implemented)
5. [Findings](#findings)
6. [Future Scope](#future-scope)
7. [Installation](#installation)
8. [Usage](#usage)
9. [Contributors](#contributors)
10. [License](#license)

---

## 📖 Overview

India, being one of the world's largest economies, has witnessed significant industrialization, urbanization, and policy shifts impacting its GHG emissions. This project explores how these factors affect emissions, captures the volatility patterns, and builds robust forecasting models to aid policymakers and researchers.

---

## 📊 Dataset

- **Source:** Publicly available datasets from governmental and international organizations.
- **Variables:**
  - Log-transformed GHG emissions.
  - GDP per capita (log-transformed).
  - Electricity production from renewable sources.
  - Manufacturing sector growth.
- **Timeframe:** 1970–2023.

---

## 🛠️ Methodology

1. **Data Preparation:**
   - Data cleaning and preprocessing.
   - Stationarity checks and log transformation.
   - Exploratory Data Analysis (EDA) to identify trends and patterns.

2. **Structural Break Analysis:**
   - Ruptures library to detect significant policy or economic event impacts (e.g., LPG reforms in 1991).

3. **Volatility Modeling:**
   - Implemented ARCH, GARCH, and EGARCH models to study volatility clustering.

4. **Forecasting Models:**
   - SARIMAX integrated with EGARCH for robust forecasting.
   - Comparative analysis with other models like VAR, exponential smoothing, and AutoARIMA.

5. **Model Evaluation:**
   - RMSE, MAE, and AIC/BIC metrics used to compare model performances.

---

## 🤖 Models Implemented

### 1. **SARIMAX (Seasonal ARIMA with Exogenous Variables):**
   - Captures seasonal trends and external influences.
   - Best model: SARIMAX(2, 0, 0) based on RMSE and AIC/BIC scores.

### 2. **GARCH/EGARCH:**
   - Modeled the conditional volatility in residuals.
   - Integrated EGARCH(1, 1) with SARIMAX for better accuracy.

### 3. **VAR (Vector Autoregression):**
   - Analyzed interdependencies between multiple time series.

### 4. **Exponential Smoothing:**
   - Simple and double exponential smoothing methods for trend analysis.

### 5. **ARIMA and AutoARIMA:**
   - Automated ARIMA modeling for baseline comparison.

---

## 🔍 Findings

1. Significant volatility spikes corresponded to major policy events, such as LPG reforms.
2. EGARCH(1, 1) captured volatility effectively and integrated well with SARIMAX.
3. SARIMAX(2, 0, 0) emerged as the most reliable forecasting model with the lowest RMSE.
4. Stationarity of the data was crucial for accurate model performance.

---

## 🚀 Future Scope

1. Explore deep learning models like LSTMs for long-term forecasting.
2. Conduct sector-wise analysis of emissions for targeted policymaking.
3. Build a user-friendly dashboard for real-time data visualization and prediction.

---

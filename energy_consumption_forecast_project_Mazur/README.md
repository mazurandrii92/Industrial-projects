# ⚡ Energy Demand Forecasting for the PJME Region  
*Optimizing Power Generation with Predictive Analytics*

## Overview

Accurate electricity demand forecasting is essential for energy providers seeking to improve operational efficiency, reduce costs, and ensure grid stability. This project presents a data-driven approach to forecast monthly electricity consumption in the **PJME** region using two industry-recognized time series models: **SARIMAX** and **Prophet**.

Our analysis provides actionable insights for **energy companies**, **grid operators**, and **policy planners** aiming to make informed decisions about production, supply planning, and infrastructure investments.

---

## Business Problem

Energy providers must balance electricity generation with fluctuating demand to avoid waste, blackouts, and unnecessary costs. Overestimating demand leads to surplus generation, while underestimating it can result in service disruption.

This project answers a key business question:

> **“How can we accurately predict regional electricity demand to support efficient power generation and grid management?”**

---

## Solution Approach

We leverage historical energy consumption data from the PJME region and apply two robust forecasting models:

- **SARIMAX**: Captures seasonality, trends, and external factors in demand patterns.
- **Prophet**: A model by Meta (Facebook) designed for business time series data with strong seasonal effects.

Both models are trained and compared to identify the optimal forecasting solution based on key performance metrics.

---

## Methodology

### 1. **Data Preparation**
- Cleaned missing values
- Extracted temporal features (e.g., month, year, seasonality)
- Split the data into training and testing sets

### 2. **Model Development**
- Configured and trained SARIMAX and Prophet models
- Tuned model hyperparameters for best performance
- Integrated custom regressors (calendar effects, holidays)

### 3. **Model Evaluation**
Forecasting accuracy was measured using:

- 📉 **MAPE** (Mean Absolute Percentage Error)
- 📉 **MAE** (Mean Absolute Error)
- 📉 **RMSE** (Root Mean Squared Error)
- 📈 **R² Score** (Goodness of fit)

### 4. **Results & Insights**
- SARIMAX outperformed Prophet with lower forecasting error and better seasonal adaptability
- Business-ready visualizations highlight trends and anomalies for planning decisions

---

## Business Value

✅ **Cost Efficiency**: Reduce unnecessary energy production through accurate demand prediction  
✅ **Grid Reliability**: Improve operational planning and mitigate blackout risks  
✅ **Scalability**: Model framework adaptable to other regions or countries  
✅ **Deployment-Ready**: Ideal for integration with BI tools or real-time energy dashboards

---

## Deliverables

- 📊 Jupyter Notebook with full modeling pipeline
- 📁 Clean and structured dataset (source: PJM)
- 📈 Forecast comparison plots and evaluation summary
- 📄 Business-focused insights and model recommendations

---

## Next Steps

- 🔌 Deploy as an API for integration with energy planning platforms
- 📈 Extend model to include weather, economic, or policy data
- 🌎 Apply to other regional energy markets for broader impact

---

## Technologies Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Statsmodels (SARIMAX)
- Facebook Prophet
- Scikit-learn

---

## Author

**Andrii Mazur**  
*Data Scientist | Energy Analytics Enthusiast*  
[GitHub Portfolio](https://github.com/mazurandrii92)
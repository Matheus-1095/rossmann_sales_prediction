# Rossmann Sales Prediction

# 📊 Rossmann Sales Prediction

**Sales forecasting for up to 6 weeks for the Rossmann pharmacy chain**, focused on cost reduction and financial impact.

- Reduced average prediction error from **36% to 4.65%** (a 31pp drop).
- Estimated gain: **€19 million in additional revenue per month**, using Kaggle data.

---

## ✅ Table of Contents

1. [Context & Motivation](#context--motivation)  
2. [Project Achievements](#project-achievements)  
3. [Architecture & Technologies](#architecture--technologies)  
4. [Data Flow](#data-flow)  
5. [Results & Metrics](#results--metrics)  
6. [How to Run](#how-to-run)  
7. [Repository Structure](#repository-structure)  
8. [Contributing](#contributing)  
9. [Contact](#contact)

---

## Context & Motivation

Rossmann operates thousands of stores across Europe and needs better sales forecasts to manage inventory, promotions, and operational planning. The primary goal of this project is:

- Build a robust **6-week sales forecasting model** using historical data (promotions, competitors, holidays, seasonality).
- Integrate the model into a production architecture via **REST API (Flask)** and **Telegram bot** for user interaction.

---

## Project Achievements

- Reduced **MAPE** from 36% to just **4.65%**, enabling significant cost savings.
- Estimated business impact: **€19 million/month in additional revenue**.
- Successfully used **XGBoost Regressor**, enhanced with Boruta for feature selection.

---

## 🛠 Architecture & Technologies

- **Languages & Data Science**: Python, Pandas, Numpy, Seaborn, Scipy, Scikit‑Learn  
- **Modeling & Feature Selection**: Boruta  
- **ML Model**: XGBoost Regressor  
- **Interactive Environment**: Jupyter Notebooks (Anaconda)  
- **Infrastructure**: Render Cloud  
- **Backend**: Flask API  
- **Communication**: Telegram Bot API

---

## 🔄 Data Flow

1. **Data cleaning and preparation** from Rossmann + competitor + holiday datasets  
2. **EDA and feature engineering** (promotions count, competition distance, etc.)  
3. **Feature selection** via Boruta to improve performance and prevent overfitting  
4. **Model training** using XGBoost and evaluation with metrics (MAPE, RMSE, etc.)  
5. **Deployment** via Flask REST API  
6. **Prediction automation** through Telegram Bot integration

---

## 📈 Results & Metrics

| Metric                   | Before | After     |
|--------------------------|--------|-----------|
| **Mean Error (MAPE)**    | 36%    | **4.65%** |
| **Financial Impact**     | —      | €19M/mo   |
| **Forecast Horizon**     | 6 wks  | 6 wks     |

---  

## 📁 Repository Structure
📦 rossmann_sales_prediction
├── notebooks/             # EDA, feature engineering, ML training
├── app.py                 # Flask prediction API
├── telegram_bot.py        # Telegram bot interface
├── environment.yml
├── requirements.txt
├── src/                   # Helper functions and pipeline code
└── README.md


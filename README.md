# 🛍️ U.S. Monthly Retail Sales Forecasting

This repository contains **Version 1 and Version 2** of a time series forecasting project on U.S. retail trade sales.

- **📘 Version 1 (V1)**: Traditional SARIMA-based modeling (in this repo)
- **🚀 Version 2 (V2)**: Advanced modeling with Auto ARIMA, Prophet, and Ensemble  
  🔗 [View V2 on Kaggle →](https://www.kaggle.com/code/vaisharma/u-s-monthly-retail-trade-sales-forecasting-v2)

---

## 🔍 Project Objectives

- Analyze historical U.S. retail sales trends (Jan 1992 – Sep 2019)
- Model and forecast 12 months of future sales
- Compare and evaluate:
  - SARIMA (manual tuning)
  - Auto ARIMA (automated tuning)
  - Prophet (Facebook's open-source model)
  - Ensemble (weighted average of multiple models)
- Generate actionable insights for business planning and demand forecasting

---

## 📊 Dataset

- **Source:** U.S. Monthly Retail Trade Sales
- **Time Range:** Jan 1992 – Sep 2019
- **Frequency:** Monthly (`MS`)
- **Target Column:** `value` (monthly retail trade sales)

---

## 🧠 Modeling Approaches

### ✅ V1: Traditional SARIMA Modeling
- Stationarity check with ADF test
- Differencing to stabilize mean
- Manual SARIMA model selection based on AIC and test RMSE
- Forecasted 12 months ahead
- Achieved **Test RMSE: ~4806.60**

### 🚀 V2: Advanced Models and Ensemble
- **Auto ARIMA:** Selected optimal (p,d,q)(P,D,Q,s) using AIC
- **Prophet:** Captured trend and seasonality with holiday-insensitive modeling
- **Ensemble:** Weighted average (0.5 * Prophet + 0.25 * SARIMA + 0.25 * Auto ARIMA)
- Achieved **lower RMSE: ~4416.12**

📘 [V2 Full Notebook (Kaggle Link)](https://www.kaggle.com/code/vaisharma/u-s-monthly-retail-trade-sales-forecasting-v2)

---

## ✅ Model Evaluation

| Model        | Test RMSE |
|--------------|-----------|
| SARIMA       | 4806.60   |
| Auto ARIMA   | 4671.98   |
| Prophet      | 4570.11   |
| Ensemble     | **4416.12** ✅ |

- Ensemble improved accuracy and generalization.
- Forecasts showed strong seasonal trends, especially peaking around Q3 months.
- Confidence intervals were visualized for uncertainty estimation.

---

## 📈 Visualizations

- Trend + Seasonality decomposition
- ACF/PACF plots for model diagnostics
- Forecast vs Actual comparison (train/test split)
- Final 12-month forecast (Oct 2019 – Sep 2020)
- Confidence intervals for risk-based planning

---

## 📦 Tech Stack

- Python
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `statsmodels` (SARIMA, Auto ARIMA)
- `prophet` (Facebook's time series model)
- `scikit-learn` (RMSE evaluation)

---

## 🧠 Business Insights

- Seasonal surges in retail sales occur around **July to September**, possibly driven by back-to-school and early fall promotions.
- Accurate sales forecasts help companies like Uber, Amazon, and Walmart:
  - Optimize staffing and inventory
  - Plan pricing strategies
  - Adjust marketing during peak/off-peak cycles
- Ensemble forecasts provide **more stable and realistic projections** by reducing individual model biases

---

## 🏁 Conclusion

This project showcases both traditional (SARIMA) and modern (Prophet, Auto ARIMA, Ensemble) approaches to time series forecasting. It demonstrates **how ensemble modeling leads to more robust forecasts**, making it ideal for business-critical use cases involving seasonality, like retail, logistics, and transportation.

📘 For advanced modeling (V2), check out the [Kaggle Notebook here](https://www.kaggle.com/code/vaisharma/u-s-monthly-retail-trade-sales-forecasting-v2).

---

## 🔗 Author

**Vaibhav Sharma**  
- [Kaggle](https://www.kaggle.com/vaisharma)  
- [Linkedin](https://www.linkedin.com/in/vaibhavsharma16/)  

📌 Based on Kaggle dataset: *U.S. Monthly Retail Trade Sales*  
🔗 Original analysis available in:
- V1: [Notebook here](https://www.kaggle.com/code/vaisharma/u-s-monthly-retail-sales-forecasting)
- V2: [Advanced Forecasting here](https://www.kaggle.com/code/vaisharma/u-s-monthly-retail-trade-sales-forecasting-v2)

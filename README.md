# Retail Sales Forecasting using SARIMA

📈 This project demonstrates a complete time series forecasting workflow using monthly U.S. retail sales data. The goal is to build a model that captures seasonal patterns and forecasts future sales — a skill highly relevant to data science roles in industries like e-commerce, logistics, and mobility (e.g., Uber).

---

## 🔍 Project Objectives

- Explore trends and seasonality in retail sales data.
- Apply SARIMA (Seasonal ARIMA) modeling for time series forecasting.
- Evaluate model performance on test data.
- Generate a 12-month forecast with confidence intervals.

---

## 📊 Dataset

- **Source**: U.S. Monthly Retail Trade Sales  
- **Time Range**: Jan 1992 – Sep 2019  
- **Frequency**: Monthly (`'MS'`)

Each record includes:
- `date`: month and year
- `value`: retail trade sales amount

---

## 🧠 Modeling Approach

- Checked for stationarity with ADF test.
- Differenced series to make it stationary.
- Evaluated multiple SARIMA models with different orders and seasonal parameters.
- Chose the best model based on lowest AIC and RMSE on test set.

---

## ✅ Model Performance

- **Test RMSE**: ~4806.60
- Accurate 12-month predictions on test set (Oct 2018 – Sep 2019)
- Final model trained on full data, used for 12-month future forecast

---

## 📈 Forecast Output

- Shows clear seasonal patterns.
- Confidence intervals capture uncertainty.
- Useful for demand planning and strategic business decisions.

---

## 📦 Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- `statsmodels` (SARIMAX)

---

## 🏁 Conclusion

The SARIMA-based forecasting model demonstrates strong predictive performance and is ideal for time series problems involving seasonality. This project is aligned with real-world applications such as forecasting rider demand, revenue, or logistics needs — key areas for Data Scientists.

---

## 🔗 Author

**Vaibhav Sharma**  
GitHub: [vaisharma16](https://github.com/vaisharma16)  
Kaggle: [vaisharma](https://www.kaggle.com/vaisharma)  
Medium: [@vai_sharma](https://medium.com/@vai_sharma)

📌 This project is based on a Kaggle dataset titled "U.S. Retail Sales (Monthly)", and the complete analysis is documented in my [Kaggle Notebook](https://www.kaggle.com/code/vaisharma/u-s-monthly-retail-trade-sales-forecasting).

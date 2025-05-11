# 📈 Bitcoin Price Forecasting Using ARIMA and SARIMA

This project aims to forecast the closing price of Bitcoin using time series analysis techniques—specifically the ARIMA and SARIMA models. Bitcoin is a highly **volatile and seasonal** market, making it a perfect candidate for time series modeling. The project also includes visual analysis and an interactive user interface built using **Streamlit**.

---

## 📊 Project Overview

- **Data Source:** Yahoo Finance (Bitcoin historical price data)
- **Time Period:** January 2023 to January 25, 2023
- **Models Used:**
  - **ARIMA (Auto-Regressive Integrated Moving Average):**
    - Suitable for non-seasonal data with trends.
  - **SARIMA (Seasonal ARIMA):**
    - Extends ARIMA by capturing seasonal effects in volatile financial data like Bitcoin.

---

## 🧪 Model Evaluation Metrics

| Model  | MAE        | MSE           | MAPE (%) | R² Score |
|--------|------------|---------------|----------|----------|
| ARIMA  | 18,695.91  | 564,851,100   | 20.16%   | -1.3965  |
| SARIMA | 14,663.09  | 359,822,600   | 15.75%   | -0.5266  |

> Although SARIMA performs better overall based on the error metrics, ARIMA occasionally gives more accurate predictions due to its simplicity.

---

## 📉 ADF (Augmented Dickey-Fuller) Test

- **Test Statistic:** 0.29
- **Conclusion:** The data is **non-stationary**, which is expected in raw financial time series.
- Models like ARIMA/SARIMA require differencing to make the series stationary, which has been applied accordingly.

---

## 🛠 Tools and Technologies

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- scikit-learn for error metrics
- statsmodels for ARIMA/SARIMA
- **Streamlit** for creating a visual web app
- Google Colab for model training and experimentation

---

## 🎥 Demo Video

Click below to watch the walkthrough of the project:

🔗 [Watch Project Demo on Loom](https://www.loom.com/share/5be6a320f24547f6b94f52915923406c)

---

## 📁 Repository Structure


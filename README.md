<img width="600" height="600" alt="walmart-logo-vector" src="https://github.com/user-attachments/assets/a8bcb968-ded5-4a26-9cdb-d326437512c8" />

# 📊 Walmart Stock Price Analysis (2025)

## 📝 Introduction

Walmart Inc. (WMT) is a retail giant whose stock price reflects broader consumer behavior and economic trends. This project analyzes Walmart’s 2025 stock data using statistical and time series modeling to derive investment insights and predict future price movements.

---

## 📂 Dataset Features

* 📅 **Date** – Trading day
* 🟢 **Open Price** – Price at market opening
* 🔼 **High Price** – Highest price of the day
* 🔽 **Low Price** – Lowest price of the day
* 🔴 **Close Price** – Price at market close
* 📉 **Adjusted Close** – Adjusted for splits/dividends
* 📈 **Volume** – Total shares traded
* 💰 **Dividends** – Shareholder payouts
* 🔄 **Stock Splits** – Split history

---

## 🎯 Objective

Train statistical time series models (ARIMA, SARIMA) to forecast Walmart's stock price and analyze performance using real data.

---

## 🛠️ Libraries Used

```python
numpy, pandas, matplotlib, seaborn  
statsmodels (ARIMA, SARIMAX), sklearn (mean_squared_error)
```

---

## 📊 Exploratory Data Analysis

* ✅ Line plot of Close prices over time
* ✅ Moving Averages (50-day, 200-day) for trend tracking
* ✅ Daily Returns and Volatility computation
* ✅ Correlation heatmap among numerical variables
* ✅ Seasonal decomposition using statsmodels

---

## 🔁 Stationarity Testing

* ADF Test on raw and differenced series
* Applied log and diff transformations to stabilize variance and achieve stationarity

---

## 🔮 Time Series Modeling

### ARIMA & SARIMA

* Applied on log-transformed series
* Initial models performed poorly on long-term forecasting
* Used RMSE as performance metric:

  ```
  ARIMA RMSE: ~0.18  
  SARIMA RMSE: ~0.36
  ```

---

## 🔄 Rolling Window Forecasting

* Rolling forecast with 100-day windows
* RMSE recalculated for each window
* Results show improved tracking of trends, but long-term predictions remain unreliable

---

## 📉 Key Takeaways

* 📌 Moving averages and decomposition provide strong insights into trends
* 📌 Statistical models like ARIMA/SARIMA struggle with long-term volatility in stock data
* 📌 Short-term forecasts using rolling windows offer better performance
* 📌 Further improvement could involve LSTM/GRU or transformer-based deep learning models

---

## 🧠 Future Scope

* Integrate LSTM for non-linear pattern prediction
* Include external macroeconomic indicators
* Build a dashboard for real-time monitoring

---

## 📁 Project Structure

```
├── walmart_stock_prices.csv  
├── walmart_analysis.ipynb  
└── README.md


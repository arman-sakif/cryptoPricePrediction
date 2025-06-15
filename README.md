# 📈 Crypto Price Prediction – Predicting Bitcoin’s High Value

This project leverages historical data from **CoinMarketCap** to predict **Bitcoin’s 'high' price** using **Linear Regression**. Designed as a practical application of data preprocessing, feature engineering, and supervised learning, the project delivers foundational insights for crypto investors and enthusiasts.

---

## 🛠️ Built With

- 🐍 Python
- 📦 Pandas, NumPy
- 📊 Scikit-learn
- 📉 Matplotlib / Seaborn (optional for visualization)

---

## 🎯 Objective

To predict Bitcoin's **daily high value** using historical market data through:
- Data cleaning & transformation
- Feature engineering
- Simple but interpretable ML modeling with **Linear Regression**

---

## 🧠 Core Idea

The model takes multiple market indicators (open, low, close, volume, market cap) and date (converted to ordinal) to predict the "high" value for a given day.

---

## 🗃️ Dataset

- Source: CoinMarketCap (historical Bitcoin price data)
- Features used:
  - `date_ordinal` (converted from calendar date)
  - `open`, `low`, `close` prices
  - `volume`
  - `marketCap`
- Target variable: `high`

---
## To make a prediction:
```python
new_data_point = pd.DataFrame({
    'date_ordinal': [date_ordinal],
    'open': [70759],
    'low': [68507],
    'close': [69342],
    'volume': [36188381096],
    'marketCap': [1366686633129]
})

predicted_high = model.predict(new_data_point)
print(f"Predicted 'high' for {tomorrow_date}: {predicted_high[0]}")
```




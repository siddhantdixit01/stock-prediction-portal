# 📈 Stock Prediction Portal

This is a stock prediction web application built using **Django (DRF)** for the backend and **React.js** for the frontend. It uses a **Long Short-Term Memory (LSTM)** model powered by **Keras** to predict stock prices based on historical data and moving averages.

🔗 **Live Preview**: [https://stock-prediction-portal-cyan.vercel.app/](https://stock-prediction-portal-cyan.vercel.app/)


## 🧠 Features

- 📊 Fetches 10 years of historical stock data using Yahoo Finance.
- 🔮 Predicts stock prices using a trained **LSTM model**.
- 📉 Displays:
  - Closing price chart
  - 100-day moving average
  - 200-day moving average
  - Predicted vs actual price chart
- 📁 Media file support for plots (served via Django).
- 📦 Deployed on **Render (Backend)** and **Vercel (Frontend)**.


## 🛠️ Tech Stack

### Frontend:
- React.js
- Axios
- Tailwind CSS

### Backend:
- Django Rest Framework
- Keras + TensorFlow
- yFinance (to fetch stock data)
- Matplotlib
- Scikit-learn
- Pandas, NumPy


## 🚀 How It Works

1. User enters a stock ticker (e.g., `GOOG`).
2. Backend:
   - Downloads 10 years of data from Yahoo Finance.
   - Processes the data.
   - Generates plots for historical and moving averages.
   - Uses pre-trained LSTM model (`.keras` file) to make predictions.
3. Returns:
   - Base64 image URLs
   - MSE, RMSE, and R² metrics

---


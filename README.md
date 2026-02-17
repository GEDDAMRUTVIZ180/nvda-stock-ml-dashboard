# 📈 NVIDIA Stock Prediction Dashboard

An end-to-end Machine Learning powered stock prediction and backtesting system built using Alpaca API, Random Forest Regression, and Streamlit.

---

## 🚀 Live Demo

🔗 [Live App Here](https://2shunxjf8r6s94mc9q9tmy.streamlit.app/)

---

## 📌 Project Overview

This project builds a production-style ML pipeline that:

- Fetches real-time NVIDIA (NVDA) stock data via Alpaca API
- Engineers financial indicators (Moving Averages, Volatility, Returns)
- Trains a Random Forest Regression model
- Predicts next-day closing price
- Generates Buy/Sell trading signals
- Performs historical backtesting
- Compares strategy performance vs Buy & Hold
- Deploys an interactive dashboard using Streamlit

---

## 🧠 Machine Learning Approach

### Feature Engineering
- Daily Returns
- Rolling Volatility (5-day)
- Moving Averages (5, 10, 20)
- Volume

### Model
- RandomForestRegressor
- 300 trees
- Max depth 10
- Time-series aware train-test split (no shuffle)

### Evaluation
- Mean Absolute Error (MAE)
- Strategy Return %
- Buy & Hold Return %

---

## 📊 Dashboard Features

- 📈 Next-day predicted close
- 📉 Actual vs Predicted price visualization
- 💰 Backtesting performance comparison
- 📊 Strategy vs Buy & Hold cumulative returns

---

## 🏗️ Project Structure

nvidia_stock_predictor/
│
├── model/
│ ├── train_model.py
│ └── model.pkl
│
├── utils/
│ └── data_loader.py
│
├── app.py
├── requirements.txt
└── README.md


---

## 🔐 Environment Setup

Create a `.env` file:

APCA_API_KEY_ID=your_key_here
APCA_API_SECRET_KEY=your_secret_here



---

## 📈 Backtesting Strategy Logic

If predicted_price > current_price → BUY  
Else → Stay in cash  

Strategy performance is evaluated using cumulative returns compared to Buy & Hold.

---

## 🔥 Future Improvements

- Add RSI, MACD indicators
- Add LSTM / Transformer models
- Walk-forward validation
- Hyperparameter tuning (Optuna)
- Deploy Docker container
- CI/CD pipeline

---

## 👨‍💻 Author

Built by Geddam Rutviz  
B.Tech Computer Science @ IIITDM Kancheepuram  
Interested in Full Stack Development, Machine Learning & Data Science
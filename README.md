# Stock Price Prediction using LSTM

A time-series forecasting pipeline that predicts future stock prices using **LSTM networks** on historical data from **S&P 500** and **NSE (HDFC Bank)**.

## Features
- **Data**: 15 years of daily OHLCV data (via `yfinance`)
- **Features**: Lagged prices/volume, weekday seasonality, SMA (5–200), MACD (12,26,9)
- **Model**: Linear Regression (baseline) + LSTM (for sequence modeling)
- **Evaluation**: Directional accuracy (85%) on out-of-sample test set

## Results
On HDFC Bank (NSE):
- **Buy-and-hold return**: +15.1%  
- **Algo-trading return**: +22.3%  
- **Model**: Outperformed benchmark by 7.2% over 365 days

## How to Run
1. Install: `pip install yfinance pandas scikit-learn matplotlib`
2. Run: `python stock_prediction.py`

> Part of my B.Tech research at DY Patil University (2024)

Stock Price Prediction Using Machine Learning (Indian Market)
📌 Project Overview

This project investigates the effectiveness of supervised machine learning models for predicting stock closing prices in the Indian stock market. The study focuses on the top 250 most actively traded companies listed on the National Stock Exchange (NSE) and evaluates model performance across different market conditions, including periods of high volatility.

The project compares ensemble and baseline models to identify the most reliable approach for financial time-series forecasting.

🎯 Objectives

To predict next-day stock closing prices using historical market data

To evaluate and compare Random Forest, XGBoost, and Decision Tree models

To analyze model performance using RMSE, MAE, and R² metrics

To study model behavior during volatile and extreme market periods

📊 Dataset

Source: Yahoo Finance (via yfinance Python library) and NSE Bhavcopy

Market: National Stock Exchange (India)

Time period: 2006 – 2025

Stocks: Top 250 most actively traded NSE-listed companies

Frequency: Daily

Features include:

Open, High, Low, Close, Adjusted Close, Volume

Technical indicators:

Simple Moving Average (SMA)

Exponential Moving Average (EMA)

Relative Strength Index (RSI)

MACD

Bollinger Bands

Average True Range (ATR)

⚙️ Methodology

Data collection using yfinance

Data preprocessing and cleaning

Feature engineering using technical indicators

Chronological train–test split (80% train, 20% test) to prevent data leakage

Model training and evaluation

Hyperparameter tuning using time-series-aware validation

Performance comparison and residual analysis

🤖 Machine Learning Models

Decision Tree Regressor (Baseline model)

Random Forest Regressor

XGBoost Regressor

📈 Evaluation Metrics

Root Mean Squared Error (RMSE)

Mean Absolute Error (MAE)

Coefficient of Determination (R²)

🏆 Key Results

Random Forest achieved the lowest prediction errors and highest stability across most stocks

XGBoost showed competitive performance but was more sensitive to short-term volatility

Decision Tree exhibited poor generalization and higher variance

Ensemble models significantly outperformed the baseline approach\

How to Run the Project

Clone the repository

Install required packages:
pip install pandas numpy scikit-learn xgboost yfinance matplotlib seaborn ta
Open the notebook:
jupyter notebook final_datascience_Project.ipynb
run cells sequentially to reproduce results

Limitations

Stock markets are inherently unpredictable

Sudden geopolitical and macroeconomic events reduce forecasting accuracy

Models are trained on historical data and may not generalize perfectly to future regimes

Future Work

Implement deep learning models such as LSTM

Incorporate sentiment analysis from news and social media

Explore volatility-specific models (e.g., GARCH)

Deploy the model as a real-time prediction application

References

Yahoo Finance

NSE Bhavcopy Archives

Breiman (2001) – Random Forest

Fischer & Krauss (2018) – LSTM for financial markets

Author

Somraj Bharadwaj Cheppela
23032481
MSc Data Science
University of Hertfordshire

Disclaimer
This project is for academic and research purposes only and does not constitute financial or investment advice.

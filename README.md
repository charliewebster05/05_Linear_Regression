# Linear Regression Trading Model – NVIDIA (NVDA)

This project implements a simple linear regression-based trading strategy to predict next-day returns for NVIDIA Corporation (NVDA) using historical stock data. The model is trained on lagged return features and generates predictive signals that can be used to simulate a basic long/short trading strategy.

# Overview:

Asset: NVIDIA (Ticker: NVDA)
Model: Linear Regression using scikit-learn
Objective: Predict next-day log returns
Features: Lagged returns (e.g., previous day's return)
Data Source: Yahoo Finance (via yfinance Python library)
Workflow:

# Download historical adjusted closing prices for NVDA.
Compute daily log returns and create lagged return features.
Split the data into training and testing sets.
Train a linear regression model on the training set.
Predict returns on the test set and generate trading signals.
Backtest strategy performance by comparing cumulative returns against a buy-and-hold benchmark.
Results:

The strategy serves as a baseline for return prediction using a simple linear model. While performance may be modest due to the simplicity of the inputs, this project provides a foundation for exploring more advanced models, feature engineering, and risk management techniques.

# Next Steps:

Add more features (volatility, momentum, volume).
Incorporate rolling window retraining.
Compare with other models (e.g., logistic regression, tree-based models).
Introduce trade filters (e.g., moving averages, volatility thresholds).
Add realistic backtesting assumptions (transaction costs, slippage).

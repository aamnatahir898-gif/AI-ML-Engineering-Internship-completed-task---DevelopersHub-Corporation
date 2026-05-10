Stock Price Prediction using Machine Learning
Project Overview
This project aims to predict the next day's closing price of a specific stock (AAPL) using historical data. It utilizes the Random Forest Regressor model to analyze price trends and volume to provide accurate forecasts. This project is a practical implementation of Time Series forecasting and Regression analysis.
Key Features
Real-time Data Fetching: Uses the yfinance library to download historical market data directly from Yahoo Finance.
Feature Engineering: Implements data shifting techniques to create a "Next Day" target variable for supervised learning.
Robust Modeling: Leverages the Random Forest algorithm, which is effective in handling non-linear relationships in financial data.
Performance Visualization: Includes a comparative plot of Actual vs Predicted prices to evaluate model reliability.
Tech Stack
Language: Python
Libraries
Pandas: Data manipulation and analysis.
Scikit-learn: Model training, splitting, and evaluation.
yfinance: Stock market data retrieval.
Matplotlib: Data visualization.
Dataset Information
The model is trained on Apple Inc. (AAPL) data from January 2022 to January 2024. The features used for prediction include: Open Price High Price Low Price Trading Volume
Target Variable: The Closing Price of the subsequent trading day.
Model Performance The model was evaluated using the Mean Absolute Error (MAE) metric.
Mean Absolute Error: ~2.18 (This indicates that on average, the prediction is within $2.18 of the actual price)
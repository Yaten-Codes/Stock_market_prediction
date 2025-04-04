# Stock_market_prediction
Project for understanding machine learning and trend on stock market using different algorithms of machine learning.
* Automated financial data pipelines using yfinance and feature engineering (lagged returns, RSI, volatility metrics) along with other technical indicators.


First I will start with a regression to get familiar with technical indicators and intro to machien learning.

Findings: <br/>
* It is very easy to overfit the model using several technical indicators,
* Using lagged days as features to predict the percent rather then price was better
* Linear Regression is overall not very good for future prediction as stocks are not linear and are affected by many factors.


Using a LightGBM-based forecasting model to predict 5-day stock returns
* hyperparameter tuning and dynamic feature selection (top 3 importance-based features)

** Model Evaluation:** Achieved <5% MAPE on price predictions and ~60% directional accuracy using walk-forward validation for select liquid stocks (results vary by stock).

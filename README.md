# 📈 Stock Price Forecasting with LightGBM

This repository contains a complete workflow for forecasting stock prices using LightGBM, a high-performance gradient boosting framework. The project was developed to compare different feature-based models on directional accuracy and MAPE (Mean Absolute Percentage Error), with a focus on enhancing financial decision-making through machine learning.

## 🧠 Project Summary

In this notebook-driven project, I implement and evaluate three predictive models to forecast short-term stock movements:

1. **Top 3 Model** – A LightGBM Regressor trained using the three most important technical indicators.
2. **Full Model** – A LightGBM Regressor trained on all engineered technical indicators.
3. **Hybrid Model** – A combination of a classifier and a regressor trained on the top five features. The classifier predicts direction (up/down), and the regressor estimates price.

Each model is evaluated based on:
- **MAPE** for price prediction accuracy
- **Directional Accuracy** for correct movement prediction (up/down)

## 📊 Features & Techniques

- **Technical Indicators**: RSI, MACD, Bollinger Bands, and more.
- **Modeling Framework**: LightGBM for regression and classification.
- **Custom Hybrid Approach**: Combines classification prediction with regression output for decision filtering.
- **Evaluation Metrics**: Includes per-ticker tables of actual vs predicted values, visualizations, and summary metrics for recent trading days.

## 🧪 Workflow Overview

1. **Data Loading**: CSVs of stock data with calculated indicators.
2. **Feature Selection**: Feature importance using built-in LightGBM metrics.
3. **Model Training**: Three separate LightGBM models.
4. **Prediction & Evaluation**: Next 5-day price prediction, accuracy metrics, and visual comparison.
5. **Exporting Results**: Prediction tables are saved per ticker with naming conventions like `ticker_April11-17.csv`.

## 📁 Example Output File Structure


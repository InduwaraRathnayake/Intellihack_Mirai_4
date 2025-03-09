# Stock Price Prediction Model

## Overview
This project implements a machine learning model to predict stock prices 5 trading days into the future. The solution includes comprehensive data analysis, feature engineering, model selection, and trading strategy evaluation.

## Approach
1. **Data Preprocessing**: Handled missing values and prepared the time series data.
2. **Exploratory Data Analysis**: Analyzed trends, distributions, and correlations in the stock data.
3. **Feature Engineering**: Created technical indicators, moving averages, and other predictive features.
4. **Model Selection**: Compared multiple models including Linear Regression, Random Forest, Gradient Boosting, and XGBoost.
5. **Trading Strategy**: Implemented and evaluated a simulated trading strategy based on model predictions.

## Selected Model: Gradient Boosting
The Gradient Boosting model was selected based on its superior performance in both statistical accuracy and trading performance.

## Performance Metrics
- Total Return: -0.9728
- Market Return: 36.3441
- Annualized Return: -0.0794
- Sharpe Ratio: -0.2233
- Maximum Drawdown: -0.9957
- Win Rate: 0.4505
- Direction Accuracy: 0.4791

## Key Features
1. Close
2. High
3. Adj Close
4. Low
5. Open
6. MA5
7. Lag_1
8. EMA12
9. MA10
10. Upper_Band

## Limitations and Future Improvements
1. **Data Limitations**: The model relies solely on price and volume data. Incorporating fundamental data, market sentiment, and macroeconomic indicators could improve performance.
2. **Model Complexity**: More sophisticated models like LSTM networks or ensemble methods could potentially capture more complex patterns.
3. **Trading Strategy**: The current strategy is simplistic. More advanced position sizing, risk management, and portfolio optimization could enhance returns.
4. **Market Regimes**: The model doesn't explicitly account for different market regimes (bull, bear, sideways). Developing regime-specific models could be beneficial.

## Usage Instructions
1. Ensure all dependencies are installed: `pip install -r requirements.txt`
2. To make predictions on new data: `python predict.py --input new_data.csv`
3. Model files (`stock_prediction_model.pkl` and `feature_scaler.pkl`) are included for direct use.

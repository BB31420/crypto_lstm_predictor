# Crypto Price Predictor: Multi-Asset ETH Forecast Model
A machine learning project leveraging time series data from multiple cryptocurrencies to predict short-term Ethereum (ETH) price movements.
## Overview
This project utilizes historical price data from Ethereum (ETH), Bitcoin (BTC), and Bitcoin Cash (BCH) to forecast ETH price direction in the next time interval. By incorporating data from multiple assets, we aim to capture both correlated market movements and potential lead-lag relationships between cryptocurrencies.
Technical Approach

* Feature Engineering: We create lagged features from ETH, BTC, and BCH prices to capture recent price trends and potential cross-asset influences.
* Multi-Asset Input: Utilizing BTC and BCH data alongside ETH provides a more comprehensive market context, potentially capturing both correlated market movements and unique signals from each asset.
* Classification Task: The model predicts a binary outcome (price increase or decrease), framed as a supervised learning classification problem.
* Ensemble Methods: We implement Random Forest and Gradient Boosting classifiers, leveraging their ability to capture complex, non-linear relationships in the data.
* Hyperparameter Tuning: GridSearchCV is employed for model optimization, systematically searching the hyperparameter space

## Model Performance

* Random Forest Classifier: Achieves a precision score of 0.4745, indicating moderate predictive power.
* Gradient Boosting Classifier: Currently shows a precision score of 0.0, suggesting potential issues with class imbalance or model configuration that require further investigation.

## Future Directions

* Explore feature importance to understand the relative impact of ETH, BTC, and BCH data on predictions.
* Implement more sophisticated time series models like ARIMA-GARCH or LSTM networks to better capture temporal dependencies.
* Investigate the addition of exogenous variables such as trading volume, market sentiment, or macroeconomic indicators to enhance predictive power.

# Energy-Forecasting-ML-Model

Project Overview
This project implements a machine learning model to forecast hourly energy demand using historical energy consumption data. The model leverages time-series features, lag variables, rolling statistics, and XGBoost regression to predict future energy load, demonstrating expertise in data preprocessing, feature engineering, and predictive modeling.

Dataset
Source: PJME Hourly Energy Dataset (Kaggle)
Contains hourly energy demand (MW) from the PJM region in the U.S.
Data preprocessing includes outlier removal, datetime indexing, and feature creation.

Key Features
Time-based features: day of week, hour, month, year, quarter, U.S. holidays
Lag-based features: 1 hour, 24 hours, and 168 hours (1 week) prior
Rolling statistics: 24-hour and 168-hour rolling mean and standard deviation

Modeling Approach
Algorithm: XGBoost Regressor
Cross-validation: TimeSeriesSplit (weekly, monthly, yearly splits)
Metrics: Root Mean Squared Error (RMSE) used to evaluate prediction accuracy
Hyperparameter tuning: learning rate, max depth, subsample, colsample_bytree

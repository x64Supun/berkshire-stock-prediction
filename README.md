# Berkshire Hathaway Stock Price Prediction
Predicting stock proces using Linear Regression and cross-validation
## Project Overview
This project analyzes Berkshire Hathaway stock data to predict the High Price of the stock using machine learning. The model is trained using Linear Regression, with additional exploratory data analysis to understand key trends.
### Key Highlights
+ EDA and Data Preprocessing - Skewness correction, log transformation, feature scaling
+ Model training and evaluation - Linear regression with cross validation
+ Error analysis - Residual analysis to check model performance
+ Visualization - Comparison of actual vs. predicted prices
### Objectives
The goal of this project is to
+ Perform EDA on historical stock price data
+ Apply data preprocessing techniquesa such as scaling and transformation
+ Train a linear regression model to predict the High Price of the stock
+ Evaluate the model's performance using cross-validation and error metrics
## Dataset & Preprocessing
+ Source - The dataset consists of historical [Berkshire Hathaway stock prices](https://www.kaggle.com/datasets/umerhaddii/berkshire-hathaway-stock-price-data) from 2015-2024.
+ Features used
  + Date (removed before training) 
  + Open - The price at market open
  + High - The highest price for that day (Target Variable)
  + Low - The lowest price for that day
  + Close - The price at market close, adjusted for splits
  + Adj Close - The closing price after adjustments for all applicable splits and divident distributions
  + Volume - The number of shares traded that day

Data Preprocessing steps
+ Handled missing values and removed unnecessary columns (date)
+ Standardized numerical features
+ Applied log transformation to correct skewness in Volume
+ Split the dataset into 80% trainig and 20% testing sets

## Model Training and Evaluation
### Model Selection
A Linear Regressioon model was trained using the preprocessed dataset. The dataset was split into:
+ 80% - Training set
+ 20% - Test set
The model was evaluated using cross-validation and performance metrics.
### Evaluation Metrics
The model has been evaluated using
+ Mean Squared Error
+ Mean Absolute Error
+ $R^2$ score

## Results and Discussion
### Model Performance
+ MAE - 0.6650
+ MSE - 0.8571
+ $R^2$ Score - 0.9998
+ Cross-Validation $R^2$ Score - \[0.99502386 0.99837863 0.99340353 0.9987327  0.99902684\]
+ Mean Cross-Validation $R^2$ Score - 0.9969

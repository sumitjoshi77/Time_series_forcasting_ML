# Time_series_forcasting_ML
This is a time series forecasting project to predict monthly alcohol sales. It builds Random Forest and Linear Regression models on lagged sales data, with the Random Forest achieving the best performance.

 Here is a draft project description for a GitHub repository for this time series forecasting ML code:

# Time Series Sales Forecasting

This project performs time series forecasting to predict future monthly alcohol sales based on previous months' sales data.

## Data
The sales data is loaded from the Alcohol_Sales.csv file. It contains a DATE index and sales column. The frequency is set to monthly. 

## Features
The following lagged sales features are created:
- sales_LastMonth: Sales from the previous month  
- sales_2MonthsBack: Sales from 2 months back
- sales_3MonthsBack: Sales from 3 months back

## Models
Two models are trained to forecast next month's sales:
1. Random Forest Regressor 
2. Linear Regression

Hyperparameters:
- Random Forest: 100 estimators, max features=3
- Linear regression: default parameters

## Results  
The models make predictions on the last 30 months and are evaluated using root mean squared error (RMSE). 

The Random Forest model achieves better performance with lower RMSE.  

## Usage
The main script loads data, trains models, makes predictions, and evaluates performance.

The models can be imported and used to make sales predictions on new data.

## Future Improvements
- Try different feature lag widths
- Tune hyperparameters further 
- Compare to other models (LSTM, ARIMA etc)
- Ensemble models

Let me know if you would like me to modify or add anything to this description! The goal is to provide a high-level overview of the key aspects of the project for potential users.

# Taxi_Fare_Predictor

## Project Overview
Predict the fare amount (inclusive of tolls) for a taxi ride in New York City given the pickup and dropoff locations.

## Data
https://www.kaggle.com/c/new-york-city-taxi-fare-prediction/data

## Data Description
The Data contains unique **ids** and **pickup_datetimes** for each taxi ride identifying each row in both the training and test sets. The features of the data include: 
- **pickup_longitude** - longitude coordinate of where the taxi ride started.
- **pickup_latitude** - latitude coordinate of where the taxi ride started.
- **dropoff_longitude** - longitude coordinate of where the taxi ride ended.
- **dropoff_latitude** - latitude coordinate of where the taxi ride ended.
- **passenger_count** - number of passengers in the taxi ride.

## Cleaning Data
An imputer is used to convert null values to numerical values using averages from each column. 


## Model Technique
The model is a Random Forest Regressor utilized to predict taxi fare amounts. The model validation is based on mean absolute error, mean squared error, coefficient of determination, and a cross validation test.

error=|actual−predicted|

With the MAE metric, take the absolute value of each error to measure model quality.


Calculate the mean squared error of the model predictions with a Random Forest Regressor. Average the square of the errors.


Measure the strength of the relationship between the random forest regressor model and the taxi fare amounts.

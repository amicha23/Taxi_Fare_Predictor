# Taxi_Fare_Predictor

## Project Overview
Purpose: Predict the fare amount (inclusive of tolls) for a taxi ride in New York City given the pickup and dropoff locations.
- Created a tool to estimate the fares of New York taxi rides based on locations (MAE ~ $2.40).
- Optimized Random Forest and Linear Regressors to find the best model.

## Data
https://www.kaggle.com/c/new-york-city-taxi-fare-prediction/data

## Code and Resources Used
**Packages:** pandas, numpy, sklean, matplotlib

## Data Description
The Data contains unique **ids** and **pickup_datetimes** for each taxi ride identifying each row in both the training and test sets. The features of the data include: 
- **pickup_longitude** - longitude coordinate of where the taxi ride started.
- **pickup_latitude** - latitude coordinate of where the taxi ride started.
- **dropoff_longitude** - longitude coordinate of where the taxi ride ended.
- **dropoff_latitude** - latitude coordinate of where the taxi ride ended.
- **passenger_count** - number of passengers in the taxi ride.

## Cleaning Data
After acquiring the data, I needed to clean up the categorical variables so it can be used in the model. An imputer is used to convert null values to numerical values using averages from each column. 


## Model Technique
The data is first split into train and validation sets of sets.

I tried using a two different models and evaluated them based on Mean Absolute Error, Mean Squared Error, Coefficient of Determination, and a Cross Validation Test. However, I looked most closely at the mean absolute error of the model because it is easer to interpret and there are less outliers.

The Random Forest Regressor outperformed the Linear Regressor on test and validation sets. 
- Random Forest MAE: $2.40
- Linear Regression MAE: $5.83

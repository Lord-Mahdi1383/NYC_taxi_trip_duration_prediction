# Taxi Trip Duration Prediction

## Overview
This project aims to predict the duration of taxi trips in New York City based on various features such as pickup/dropoff locations, time information, passenger count, and calculated distance. The model uses XGBoost Regressor with hyperparameter tuning to achieve optimal performance.

## Dataset
The dataset is taken from Kaggle's NYC Taxi Trip Duration competition:  
https://www.kaggle.com/c/nyc-taxi-trip-duration/data


## Project Structure
### Data Preprocessing
  - Handle missing values and duplicates
  - Convert store_and_fwd_flag to binary (0/1)
  - Feature engineering pickup and dropoff datetime

### Outlier Detection and Removal
  - pickup and dropoff coordinates
  - Trip distances
  - Trip durations
  - Passenger counts

### Model Training
  - Algorithm: XGBoost Regressor
  - Objective: reg:squaredlogerror
  - Hyperparameter Tuning: RandomizedSearchCV
  - Evaluation Metric: Root Mean Squared Log Error (RMSLE)


## Installation
### Clone The Repository
```bash
git clone https://github.com/Lord-Mahdi1383/NYC_taxi_trip_duration_prediction
cd NYC_taxi_trip_duration_prediction
```

### Install Dependencies
```bash
pip install -r Requirements.txt
```

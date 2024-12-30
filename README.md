# Rapido Bike Sharing Demand Prediction

This project aims to predict bike rental demand using machine learning models, enabling efficient inventory management and improved customer satisfaction for bike-sharing businesses.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Data Wrangling](#data-wrangling)
- [Data Visualization](#data-visualization)
- [Feature Engineering](#feature-engineering)
- [Model Implementation](#model-implementation)
- [Conclusion](#conclusion)

## Project Overview

The increasing popularity of bike-sharing programs necessitates accurate demand prediction for optimal resource allocation. This project utilizes historical bike rental data to build predictive models, considering factors like weather conditions, time of day, and special events.

## Dataset

The dataset contains hourly bike rental records along with relevant features such as:

- Date and time
- Rented bike count
- Temperature
- Humidity
- Windspeed
- Visibility
- Dew point temperature
- Solar radiation
- Rainfall
- Seasons
- Holiday
- Functional Day

## Data Wrangling

The following data wrangling steps were performed:

- Date conversion to datetime format
- Extraction of year, month, day, and weekday
- Identification of numerical, discrete, and categorical variables

## Data Visualization

Various visualizations were created to gain insights into the data, including:

- Histograms of rented bike count distribution
- Scatterplots of rides by day, month, and year
- Line plots of rented bike count by hour and season
- Scatterplots of rented bike count by temperature and humidity
- Bar charts of total rentals per day and month
- Correlation heatmap

## Feature Engineering

The following feature engineering techniques were applied:

- Handling missing values (none found)
- Handling outliers (dew point temperature removed due to high correlation with temperature)
- Categorical encoding (mapping for binary variables, one-hot encoding for nominal variables)
- Data transformation (logarithmic transformation of the target variable)
- Data scaling (StandardScaler)

## Model Implementation

Three machine learning models were implemented and evaluated:

- Linear Regression
- Random Forest Regressor
- XGBoost Regressor

Hyperparameter tuning was performed using GridSearchCV and RandomizedSearchCV.

## Conclusion

The tuned XGBoost Regressor emerged as the best performing model, achieving the lowest RMSE and highest R-squared. This model provides accurate bike demand predictions, enabling bike-sharing businesses to:

- Optimize inventory management
- Implement effective pricing strategies
- Allocate resources efficiently
- Enhance customer satisfaction

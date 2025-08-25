# Air Quality Index Prediction Using Random Forest

This project predicts the Air Quality Index (AQI) based on various air pollutant measurements using a Random Forest regression model built in Python. It uses historical Delhi air quality data containing pollutants like PM2.5, PM10, NO2, SO2, CO, and Ozone, along with the recorded AQI values.


## Project Overview

The goal is to use historical air quality data to train a machine learning model that can estimate AQI from pollutants like PM2.5, PM10, NO2, SO2, CO, and Ozone. Accurate AQI prediction helps monitor and improve environmental and public health.

## Technologies and Libraries Used

- Python
- Pandas and NumPy for data manipulation
- Matplotlib and Seaborn for visualization
- Scikit-learn for machine learning (Random Forest, metrics, train-test split)

## Data

The dataset (`airqualityindex.csv`) contains daily readings of various air pollutants, holiday counts, and the actual AQI values. The data is cleaned by dropping missing values and standardizing column names.

## Exploratory Data Analysis (EDA)

- Pair plots visualize relationships among pollutants and AQI.
- Correlation heatmap shows how different pollutants are correlated with AQI.

## Model Building and Evaluation

- Features: PM2.5, PM10, NO2, SO2, CO, and Ozone.
- Target: AQI.
- Train-test split: 80% training, 20% testing.
- Model: Random Forest Regressor with 100 trees.
- Evaluation metrics: Mean Absolute Error (~18.61), Mean Squared Error (~848.12), R2 Score (~0.93), showing strong predictive performance.

## Visualization

A comparison plot between actual and predicted AQI values (first 100 samples) is used to visually assess the model's accuracy.

## How to Use

1. Load the dataset CSV file in the same directory.
2. Run the Python code cells step-by-step for preprocessing, EDA, training, and evaluation.
3. Visualize results using the provided plots.

## Future Work

- Experiment with other regression models and hyperparameter tuning.
- Use more extensive data for improved generalization.
- Deploy the model for real-time AQI prediction.

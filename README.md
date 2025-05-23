# Air-Quality-Index-Prediction
A machine learning-based system that predicts urban air quality by analyzing key pollutants (CO, NO2, O3) using regression and time series models. It also classifies air quality as Good, Moderate, or Poor, aiding awareness and proactive health measures.

Purpose: The notebook is focused on predicting urban air quality using machine learning and time-series forecasting techniques. It processes air quality data and forecasts pollutant levels like CO (Carbon Monoxide).

Key Details:

Libraries Used: Data Manipulation & Visualization: pandas, numpy for data handling. seaborn, matplotlib for plotting. Machine Learning: sklearn for regression, model training, and evaluation. Forecasting: Prophet for time-series forecasting. Other Utilities: pickle for saving/loading models. os for file handling.
Data Handling: Loads air quality data from a CSV file (AirQualityUCI.csv). Cleans the dataset: Removes unnecessary columns. Handles missing values by replacing them with the mean.
Forecasting with Prophet: Combines date and time columns to create a datetime series. Prepares data for Prophet by creating a DataFrame with: ds: Date and time. y: CO levels (CO(GT) column). Fits the forecasting model and predicts future CO levels for 365 hours.
Visualization: Plots the forecasted data and its components using Prophet's built-in plotting methods. Uses Seaborn to create pairplots of the forecasted data. Observations: Warnings: It disables yearly seasonality in Prophet by default and provides a warning about deprecated frequency (H → h). Outputs: Visualizes forecasted values and trends. Generates plots of Prophet components and pairplots using Seaborn. Summary: This notebook is part of a machine learning-based system aimed at predicting and analyzing air quality. It uses regression and time-series forecasting to predict pollutant levels, which could help classify air quality as Good, Moderate, or Poor.

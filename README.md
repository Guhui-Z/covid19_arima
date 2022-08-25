# Time-series Analysis of U.S. Covid-19 Cases

## Project Objective
This project aims to visualize and analyze U.S. COVID-19 data in the time frame from 2020-01-21 to 2022-08-02, as well as predict the number of cases in the following 5 days.

## Methods
+ Data Cleaning
+ Data Visualization
+ Time Series Analysis 
+ Arima Model

## Technologies
+ python
+ statsmodels
+ NumPy
+ pandas
+ Matplotlib
+ plotly

## Project Description:
+ Data Source: The data are collected from the New York Times github repo https://github.com/nytimes/covid-19-data
+ Data Cleaning: 
  - Transformed the date column into the date class
  - Added the `new_cases` and `new_deaths` column
  - Calculated 7-day rolling averages of `cases`, `deaths`, `new_cases` and `new_deaths`
+ Data Visualization:
  - Double axis bar plots for U.S. cases over time
  - Animated geographical plots and racing bar plots for U.S. cases per state over time
+ Used the log-differencing technique to make the data stationary
  - Conducted the Augmented Dickey-Fuller Test and plotted autocorrelation plots to ensure stationarity.
+ Performed grid search to find the optimal ARIMA model

## Project Results:
+ Final model predicted COVID-19 cases of the following 5 days with ±1% error

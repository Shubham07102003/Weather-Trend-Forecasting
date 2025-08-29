
# PM Accelerator Weather Trend Forecasting

This repo contains a complete walkthrough for the Weather Trend Forecasting assignment using Kaggle Global Weather Repository

Mission note from the PM Accelerator website
Our mission is to break down financial barriers and achieve educational fairness. With the goal of establishing 200 schools worldwide over the next 20 years, we aim to empower more kids for a better future in their life and career, simultaneously fostering a diverse landscape in the tech industry.

## Contents

1 Jupyter notebook PMA Weather Forecasting Assessment ipynb with all steps end to end
2 This README with instructions and project notes

## Dataset

Kaggle dataset Global Weather Repository  
URL https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository

The dataset provides daily weather records for many cities world wide with more than forty fields including temperature wind pressure humidity and several air quality indicators

## What the notebook covers

1 Data loading and lightweight memory optimization
2 Time parsing and basic normalization
3 Missing value imputation per city with global fallback
4 Outlier capping through winsorization
5 Exploratory analysis for coverage trends and time plots
6 Temperature and precipitation visualizations
7 Correlation heatmap for numeric features
8 Air quality versus weather checks
9 Spatial scatter for lat lon with city averages
10 Anomaly detection using Isolation Forest
11 Forecasting for the most covered city with these models
    1 Naive last value
    2 Seasonal naive with seven day season
    3 Random Forest on lag features and calendar features
    4 SARIMAX when statsmodels is available
12 Simple ensemble that averages available model predictions
13 Validation metrics MAE RMSE MAPE and R two
14 Walk forward forecast for the next two weeks
15 Feature importance from Random Forest plus permutation importance

## How to run locally or on Kaggle

1 Open the notebook PMA Weather Forecasting Assessment ipynb
2 Ensure the CSV file is available at the path shown at the top DATA PATH or update the path
3 Run all cells from start to finish
4 The notebook will pick the city with the most data automatically and show validation results along with a fourteen day forecast

## Reproducibility choices

1 Pure matplotlib is used for charts for maximum compatibility
2 Random seeds are set for the stochastic models where supported
3 Where libraries are optional the code detects availability and continues gracefully

## Folder suggestions when you push to GitHub

1 Put the notebook at the repo root
2 Add the README at the repo root
3 If you add figures later use a folder named figs
4 If you export results use a folder named outputs

## Acknowledgment

Mission text taken from the PM Accelerator website


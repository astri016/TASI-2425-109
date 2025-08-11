# TASI-2425-109

# A Hybrid ARIMA-LSTM with Attention for Student Stress Prediction using Physiological Time-Series

## Overview

This repository contains the code and resources for the final research project that implements a hybrid forecasting model combining ARIMA and LSTM with an Attention mechanism. The model is designed to predict student stress levels using physiological time-series data such as Galvanic Skin Response (GSR), Sleep Hours, Anxiety Level, and Mood Score. The main goal is to enhance time-series forecasting accuracy by leveraging both statistical and deep learning methods, enriched with an attention layer for improved temporal feature weighting.

## Proposed Model Architecture
### Hybrid ARIMA–LSTM with Attention
* Model Components:
  - ARIMA: Utilized for modeling and forecasting stationary time-series components (e.g., GSR).
  - LSTM: Used for capturing non-linear dependencies in multivariate physiological data.
  - Attention Layer: Integrated into the LSTM model to focus on important time steps and improve prediction performance.

## Forecasting Workflow
* Data Preprocessing:
  - Handling missing values, normalization, and time-series differencing for stationarity checks.
  - Splitting data into training and testing sets based on time blocks.
* ARIMA Forecasting:
  - Using Auto-ARIMA to determine optimal p, d, q parameters.
  - Forecasting stationary univariate series (GSR).
* LSTM with Attention Forecasting:
  - Modeling non-stationary multivariate features (Sleep Hours, Anxiety Level, Mood Score).
  - Applying attention mechanism to assign higher weights to important time steps.
* Hybrid Prediction:
  - Combining ARIMA predictions (for GSR) with LSTM+Attention predictions (for other features) to produce final multi-feature forecasts.

## Fine-Tuning and Customization
* Hyperparameter Optimization:
  - Adjusting learning rate, dropout rate, batch size, and attention dimensions to minimize loss and maximize accuracy.
* Evaluation Metrics:
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
    
## Dataset
The dataset used in this research contains physiological data of students, including:
* Galvanic Skin Response (GSR)
* Sleep Duration
* Anxiety Scores
* Mood Scores
You can access the dataset [here](https://www.kaggle.com/datasets/ziya07/student-health-and-attendance-data/data).


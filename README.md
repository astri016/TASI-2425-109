# TASI-2425-109

# Hybrid ARIMA-LSTM with Attention Mechanism for Student Stress Prediction

## Overview

This repository contains the code and resources for the final research project that utilizes a hybrid ARIMA-LSTM model with an attention mechanism to predict student stress levels based on multivariate time-series data. The main goal of the project is to improve the accuracy of stress level prediction for students by integrating physiological indicators such as Galvanic Skin Response (GSR), Sleep Hours, Anxiety Level, and Mood Score. The model aims to leverage both ARIMA for capturing linear trends and LSTM with attention for non-linear and temporal dependencies in the data.

## Research Focus

The research focuses on the development of a hybrid ARIMA-LSTM model with an attention mechanism to predict student stress levels. The attention mechanism helps the model focus on the most relevant parts of the data to improve the prediction accuracy and interpretability of the model. The dataset used includes physiological data collected from students over time to understand how factors like sleep, mood, and anxiety levels influence stress.

## Features

- **ARIMA Model**: Captures linear trends and seasonal patterns in the time-series data.
- **LSTM Model**: Focuses on learning long-term dependencies and nonlinear relationships in the data.
- **Attention Mechanism**: Prioritizes the most relevant data points in the sequence to improve prediction accuracy.
- **Multivariate Time-Series Data**: Includes variables such as GSR, sleep hours, anxiety level, and mood score.
- **Student Stress Prediction**: Predicts the stress level based on historical physiological data.

## Dataset

The dataset used in this research contains physiological data of students, including the following attributes:
- **Student ID**: Unique identifier for each student.
- **Date**: Date of data recording.
- **Class Time**: The time range during which the student attended class.
- **Attendance Status**: Whether the student was present, absent, or late.
- **Stress Level (GSR)**: Stress level measured by Galvanic Skin Response (GSR).
- **Sleep Hours**: The number of hours the student slept before class.
- **Anxiety Level**: The anxiety level of the student.
- **Mood Score**: The emotional condition of the student during the class.
- **Risk Level**: Health and engagement risk category (Low, Medium, High).
  
You can access the dataset [here](https://www.kaggle.com/datasets/ziya07/student-health-and-attendance-data/data).


## Methodology

1. **Data Preprocessing**: The data is processed by handling missing values, normalizing features, and splitting it into training and testing sets.
2. **Model Development**: The ARIMA model captures linear trends, while the LSTM model captures long-term dependencies and nonlinearities. The attention mechanism is integrated to allow the model to focus on the most relevant time steps.
3. **Evaluation**: The model's performance is evaluated using metrics such as MAE (Mean Absolute Error) and RMSE (Root Mean Squared Error).

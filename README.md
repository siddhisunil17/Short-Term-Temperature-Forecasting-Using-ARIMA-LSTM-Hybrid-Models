# Short-Term-Temperature-Forecasting-Using-ARIMA-LSTM-Hybrid-Models


Overview

This project focuses on short-term temperature forecasting using statistical (ARIMA) and deep learning (LSTM) models. It compares their performance and introduces a hybrid ARIMA-LSTM model that combines the strengths of both approaches. The results are based on data from 35 major U.S. cities spanning 1948–2022, demonstrating the hybrid model's adaptability and accuracy across diverse climatic conditions.

Objectives
1. Compare ARIMA, LSTM, and hybrid ARIMA-LSTM models for short-term temperature forecasting.
2. Enhance prediction accuracy by leveraging both statistical reliability (ARIMA) and deep learning flexibility (LSTM).
3. Provide insights for industries like agriculture, energy, transportation, and urban planning.

Technologies Used
1. Languages: Python, R
2. Libraries and Frameworks: TensorFlow, Pandas, NumPy, Matplotlib, ggplot2
3. Statistical Methods: ARIMA (Auto-Regressive Integrated Moving Average)
4. Deep Learning: LSTM (Long Short-Term Memory)

Data
1. Dataset: Daily temperature records from 35 major U.S. cities (1948–2022).
2. Source: Publicly available historical weather datasets.
3. Preprocessing:
   
   a. Normalization of temperature data.
   
   b. Stationarity checks using Augmented Dickey-Fuller (ADF) test.
   
   c. Seasonal decomposition for ARIMA model preparation.


Models Implemented

ARIMA:

1. Captures linear trends and seasonality.
2. Configuration: (1,1,1) based on ADF test results.
3. Performs well in stable climates but struggles with high variability.
   
LSTM:

1. Two-layer LSTM model with dropout regularization.
2. Optimizer: Adam | Loss Function: Mean Squared Error.
3. Captures non-linear dependencies and long-term temporal relationships.
   
Hybrid ARIMA-LSTM:

1. Dynamically adjusts weights between ARIMA and LSTM based on RMSE.
2. Combines statistical precision and deep learning flexibility.
3. Achieved RMSE < 0.03 in diverse climatic conditions.

Results

1. Performance:
   
   a. Hybrid model consistently outperformed standalone ARIMA and LSTM models.

   b. Best performance in coastal cities (e.g., Honolulu, San Francisco) with stable climates.

   c. Moderate performance in regions with high variability (e.g., Phoenix, Boston).

2. Metrics: Evaluated using Root Mean Square Error (RMSE) and Mean Absolute Error (MAE).
   
   a. RMSE (Hybrid): < 0.03

   b. RMSE (LSTM): 0.03–0.05

   c. RMSE (ARIMA): 1.7–27.4

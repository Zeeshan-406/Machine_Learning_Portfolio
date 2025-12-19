# Air Quality Forecasting
## Problem Statement
The aim of this project is to predict future air quality levels using historical air pollution data
and machine learning models.
## Dataset
- Source: Kaggle
- Size: (9357, 15)
## Tools & Technologies
- Python
- Pandas, NumPy, Matplotlib
- Scikit-learn
## Algorithm Used
- Forecasting FB Prophet Algorithm
## Results
The Prophet-based time series forecasting model was trained on historical air quality data
to predict NO2 concentration levels. The model successfully captured temporal trends
and patterns in the data.
The evaluation results on the test set are as follows:
- RMSE: 34.20
- MAE: 26.74
- R2 Score: 0.39
These results indicate that the model provides reasonable forecasting performance and
can be useful for understanding air pollution trends and supporting early warning systems.
## How to Run
1. Open Google Colab
2. Install required libraries
3. Train the model
## Future Work
- Use deep learning time-series models (LSTM, Transformer)
- Support multi-pollutant forecasting
- Integrate real-time sensor data
- Deploy as a web-based air quality monitoring system


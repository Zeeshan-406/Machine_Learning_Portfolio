# FFC Stock Price Prediction using LSTM
## Problem Statement
Stock price prediction is a challenging task due to the non-linear and volatile nature of financial markets.  
This project focuses on predicting the future closing prices of **Fauji Fertilizer Company (FFC)** listed on the **Pakistan Stock Exchange (PSX)** using a **Long Short-Term Memory (LSTM)** deep learning model.
## Dataset
- **Source:** Yahoo Finance  
- **Ticker Symbol:** FFC.KA  
- **Market:** Pakistan Stock Exchange (PSX)  
- **Data Type:** Daily historical stock prices  
- **Target Feature:** Close Price  
## Tools & Technologies
- Python  
- Google Colab  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- TensorFlow / Keras  
## Data Collection
Historical stock price data was downloaded directly from Yahoo Finance using the `yfinance` library.  
The dataset includes daily prices indexed by date.
## Data Preprocessing
- Selected **Close price** for prediction  
- Normalized data using **MinMaxScaler**  
- Scaled values between 0 and 1  
## Sequence Creation
- Created time-series sequences using a **60-day sliding window**  
- Each input consists of prices from the previous 60 days  
- Output is the price of the next day  
## Train-Test Split
- 80% data used for training  
- 20% data used for testing  
- Data split was done chronologically to prevent data leakage  
## Model Architecture
- Random Forest Regressor (Accuracy was Poor)
-Prophet (Accuray was Poor)
The LSTM model consists of:
- Two LSTM layers (50 neurons each)  
- Dropout layers to reduce overfitting  
- One Dense output layer for price prediction  
## Model Training
- Optimizer: Adam  
- Loss Function: Mean Squared Error (MSE)  
- Model trained for multiple epochs to learn temporal patterns  
## Model Evaluation
Model performance was evaluated using:
- Root Mean Squared Error (RMSE)  
- Mean Absolute Error (MAE)  
## Future Price Prediction (Recursive Forecasting)
- Last 60 days of scaled data used as input  
- Model predicts the next day’s closing price  
- Predicted value is appended back into the input window  
- This recursive process is repeated to predict the next **30 future trading days**
## Visualization
- Historical stock prices plotted using actual data  
- Future predicted prices plotted alongside historical prices  
- Visualization highlights trend continuation  
## Results
- The LSTM model learned historical price patterns  
- Predicted values follow the overall market trend  
- Exact price prediction is difficult due to market volatility  
## Limitations
- Stock prices are affected by external factors such as news and economic events  
- Recursive predictions may accumulate error over time  
- Model does not include technical indicators or sentiment data  
## Future Improvements
- Add technical indicators (RSI, MACD, Moving Averages)  
- Integrate news or sentiment analysis  
- Compare performance with ARIMA and Prophet models  
- Predict price direction (Up / Down) instead of exact values  
## How to Run
1. Open Google Colab  
2. Install required libraries  
3. Run the notebook cells sequentially  
4. Train the LSTM model  
5. Generate future stock price predictions  

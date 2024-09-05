# Stock-Market-Analysis-Using-LSTM

Stock Market Analysis Using LSTM
Project Overview
This project applies Long Short-Term Memory (LSTM), a type of recurrent neural network, to perform time series forecasting on historical stock prices. By using past stock data, the LSTM model predicts future stock prices, helping analysts and investors understand trends in the market.

The project uses the Yahoo Finance API to gather stock price data and the Keras deep learning library to build and train the LSTM model.

Objective
To forecast stock prices using the LSTM model based on historical stock data.
To evaluate the performance of the LSTM model using Root Mean Squared Error (RMSE).
To visualize the predictions and compare them with actual stock prices.
Dataset
The stock price data is fetched using the Yahoo Finance API. This dataset includes the following fields:

Date: The date of the recorded stock price.
Close: The closing stock price for that day.
Example Data:
Date	Close
2022-01-01	150.00
2022-01-02	152.00
2022-01-03	155.00
The closing price is used as the target variable for time series forecasting.

Tech Stack / Libraries Used
Python: The programming language used for building the project.
Yahoo Finance API (yfinance): Used to download historical stock prices.
Keras / TensorFlow: Deep learning libraries used to build and train the LSTM model.
Matplotlib: Used to plot and visualize stock prices.
NumPy & Pandas: For numerical and data manipulation.
Scikit-learn: Used for scaling and evaluating the model.
Steps in the Project
Data Collection:

Download historical stock price data from Yahoo Finance using the yfinance library.
Data Preprocessing:

The data is scaled between 0 and 1 using MinMaxScaler.
Time series data is reshaped to create sequences of 60 time steps for the LSTM model.
Modeling:

The LSTM model is built using Keras, consisting of two LSTM layers followed by dense layers.
The model is trained to predict stock prices based on past data.
Prediction:

The model is used to predict stock prices for both the training and test datasets.
The results are visualized alongside actual stock prices.
Evaluation:

The Root Mean Squared Error (RMSE) is used to evaluate the model's performance.
Lower RMSE values indicate better model performance.
Visualizations
1. Stock Price Prediction
The actual vs predicted stock prices are visualized using Matplotlib. The green line represents training predictions, the red line represents test predictions, and the blue line represents actual stock prices.


2. Loss Plot
The loss during the training of the LSTM model is visualized to show how well the model converged.


Model Performance
The performance of the LSTM model is evaluated using Root Mean Squared Error (RMSE) on the training and testing datasets:

Training RMSE: X.XX
Testing RMSE: X.XX
Lower RMSE values indicate better model predictions.

How to Run the Project
1. Clone the Repository:
bash
Copy code
git clone https://github.com/shiva201/Stock-Market-Analysis-Using-LSTM.git
2. Install Dependencies:
You need to install the required libraries. Run the following command:

bash
Copy code
pip install yfinance numpy pandas matplotlib scikit-learn tensorflow keras
3. Run the Code:
Once the environment is set up, you can run the Python script:

bash
Copy code
python stock_market_lstm.py
4. View the Results:
The script will generate stock price predictions and plot the actual vs predicted stock prices.

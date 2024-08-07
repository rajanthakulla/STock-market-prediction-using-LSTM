This project involves prediction of stock market uisng LSTM neural network. The evaluation metrics used include Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared (R²) to assess model performance.

Requirements:
To run this project, you'll need the following Python packages: pandas, numpy, matplotlib, scikit-learn, tensorflow.

Data:
The data used in this project is in IRFC_data.csv, which includes historical stock prices with the following columns: Date: The date of the stock data, open: Opening price, high: Highest price, low: Lowest price, close: Closing price, adjclose: Adjusted closing price


Data Preprocessing:
The preprocessing.py script handles data loading, normalization, and feature engineering. It creates lag features for the close price and prepares the data for training and testing.

Model:
The model.py script defines the LSTM model architecture, compiles the model with the Adam optimizer, and trains it using historical stock price data. Early stopping is used to prevent overfitting.

Evaluation:
The evaluation.py script evaluates the model's performance using MAE, RMSE, and R². It also generates plots for actual vs. predicted prices and the training and validation loss.

Results:
The model's performance metrics are as follows:

Mean Absolute Error (MAE): 5.86
Root Mean Squared Error (RMSE): 9.12
R-squared (R²): 0.96

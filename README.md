# Stock Price Prediction Using Machine Learning

## Objective

The objective of this project is to predict the closing price of a stock using historical data and a machine learning model.

## Dataset

The project uses historical stock data from the `Stockprice.csv` file. This dataset contains information about the stock's open, high, low, close, adjusted close prices, and volume over a period of time.

## Methodology

The project follows these steps:

1.  **Load the data**: The stock data is loaded from the `Stockprice.csv` file into a pandas DataFrame.
2.  **Preprocess the data**: The data is preprocessed by handling missing values (although none were found in this specific dataset) and scaling the features using `MinMaxScaler`. The features used for prediction are 'Open', 'High', 'Low', and 'Volume'.
3.  **Split the data**: The preprocessed data is split into training and testing sets to train and evaluate the model.
4.  **Train the model**: A Random Forest Regressor model is trained on the training data.
5.  **Make predictions**: The trained model is used to make predictions on the test data.
6.  **Evaluate the model**: The model's performance is evaluated using Mean Squared Error (MSE) and R-squared (R2) score.
7.  **Visualize the results**: A scatter plot is generated to compare the actual and predicted stock prices for the test data.

## Results
![image](https://github.com/user-attachments/assets/d9a96555-a11b-4840-874a-ca478477345e)




The Random Forest model achieved a Mean Squared Error (MSE) of approximately 27.71 and an R-squared (R2) score of approximately 0.9976 on the test data. This indicates that the model performed very well in predicting the stock closing prices based on the selected features. The scatter plot visually confirms that the predicted prices are in close agreement with the actual prices.

## Key Findings

*   The dataset was successfully loaded and contained no missing values.
*   The selected features ('Open', 'High', 'Low', and 'Volume') were scaled effectively.
*   The Random Forest Regressor model demonstrated high accuracy in predicting stock prices, as indicated by the high R-squared score.

## Future Steps

*   Explore additional features that could potentially improve prediction accuracy (e.g., technical indicators, news sentiment).
*   Tune the hyperparameters of the Random Forest model to optimize its performance.
*   Compare the performance of the Random Forest model with other regression models to identify the most suitable model for this task.
*   Implement time series cross-validation for a more robust evaluation of the model's performance over time.

## How to run the code

1.  Make sure you have the `Stockprice.csv` file in the same directory as the notebook.
2.  Install the required libraries: pandas, scikit-learn, and matplotlib.
3.  Run the code cells sequentially in the provided notebook.

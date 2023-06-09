# Trading-strategies-using-Ridge-regression

## Stock Price Prediction and Trading Strategy for Service Now Stock

This code implements a stock price prediction and trading strategy using ridge regression and Bollinger Bands. It performs the following tasks:

1. Importing necessary libraries and modules:
   - yfinance: A Python library for accessing financial data from Yahoo Finance.
   - datetime: For handling date and time.
   - numpy: For numerical computations.
   - scipy.optimize: For optimization functions.
   - matplotlib: For data visualization.
   - pandas: For data manipulation and analysis.
   - seaborn: For statistical data visualization.
   - warnings: For suppressing warnings.
   - math: For mathematical functions.

2. Downloading stock price data:
   - The code downloads historical stock price data for the "NOW" stock from Yahoo Finance for the specified date range.

3. Calculating logarithmic returns:
   - The code calculates the logarithmic returns (lrets) based on the closing price of the stock.

4. Preparing the data:
   - The code calculates the Stock_Price based on the high, low, and close prices.
   - The data is rounded to four decimal places.
   - Any missing values are filled with 0.
   - The data is split into training and testing sets.

5. Implementing Ridge Regression:
   - The code defines a RidgeRegression class for ridge regression modeling.
   - It fits the model on the training data using the RidgeRegression class.
   - Grid search is performed to find the best hyperparameters using cross-validation.

6. Making predictions and evaluating the model:
   - The code predicts the stock prices for the test data.
   - Mean squared error (MSE) and root mean squared error (RMSE) are calculated to evaluate the model's performance.

7. Visualizing the predicted and actual stock prices:
   - The code plots the predicted and actual stock prices on two subplots.
   - The first subplot shows the predicted close prices.
   - The second subplot shows the actual close prices.

8. Implementing a trading strategy:
   - The code compares the predicted and actual stock prices to determine the trading actions (Buy, Sell, Hold).
   - The code keeps track of the portfolio value, amount, balance, and stocks for each trading action.
   - The trading actions, portfolio, amount, and stocks are stored in separate lists.
   - The results are printed for each trading action.

9. Calculating profit and Sharpe ratio:
   - The code calculates the profit percentage based on the initial and final amount.
   - The Sharpe ratio is calculated as a measure of risk-adjusted return.

10. Visualizing the trading strategy results:
    - The code creates a DataFrame to store the trading strategy results.
    - The DataFrame includes the actual and predicted close prices, date, trading actions, stocks, portfolio value, and amount.
    - The actual vs predicted close prices are plotted.
    - The total amount over time is plotted.

11. Visualizing Bollinger Bands:
    - The code calculates the long moving average (SMA), short moving average, upper band, and lower band using Bollinger Bands.
    - The Bollinger Bands are visualized with the actual stock price.

12. Conclusion:
    - The code provides a comprehensive trading strategy implementation using stock price prediction and Bollinger Bands.

Note: This code is for educational purposes only and should not be used for real trading without proper evaluation and consideration of risks.

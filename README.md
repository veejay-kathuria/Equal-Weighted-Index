# Portfolio Weighting Calculator

This script calculates the number of shares for each stock in a portfolio based on whether the user wants a market capitalization weighted portfolio or an equal weighted portfolio.

## Requirements
- Python 3.x
- pandas
- numpy
- requests
- xlsxwriter
- yfinance

## Installation

Install the required Python libraries using pip:
pip install pandas numpy requests xlsxwriter yfinance

## Inputs:
1. Total portfolio size in dollars.
2. File path for the CSV file containing the list of stock tickers. (example template oof CSV is given in repository).
3. Type of portfolio weighting: Market Capitalization Weighted Portfolio or Equal Weighted Portfolio.

## Portfolio Weighting Functions
The script contains two functions to calculate the number of shares for each stock based on the chosen weighting method.

## Functions
- equal_weighted_portfolio(result_df)
Calculates: The number of shares for each stock in an equal weighted portfolio.
Parameters: DataFrame containing stock information. Must include 'Market Cap' and 'Last Price' columns.
Returns: DataFrame with an added 'Number of Shares' column indicating the number of shares for each stock in the equal weighted portfolio.

- mcap_weighted_portfolio(result_df)
Calculates: The number of shares for each stock in an equal weighted portfolio.
Parameters: DataFrame containing stock information. Must include 'Market Cap' and 'Last Price' columns.
Returns:  DataFrame with added columns 'Weight', 'Dollar Amount Allocated', and 'Number of Shares' indicating the weight, dollar amount allocated, and number of shares for each stock in the market cap weighted portfolio.

## License
This project is licensed under the MIT License.

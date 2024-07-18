# Stock Analysis Readme

## Overview
This Python script is designed to analyze historical stock prices and visualize them with moving averages and Bollinger Bands. It also extracts key financial figures for a specified list of stock tickers. I use it to have an overview of the few equities that I'm having a continuous look at. Historic prices are important for me to take into account. I simply want to know how the prices have moved historically.

## Requirements
To run the script, you need to have the following Python packages installed: yfinance, pandas, matplotlib, and seaborn. You can install these packages using pip.

## Script Description

### Importing Packages
The script begins by importing the necessary packages, including yfinance for retrieving stock data, pandas for data manipulation, matplotlib for plotting, and seaborn for enhanced visual styles.

### Function Definition
The core function, `plot_stock_with_indicators`, takes a stock ticker as input and performs several tasks. It retrieves historical stock prices for the past year, calculates the 20-day moving average (MA20) and Bollinger Bands, and replaces any infinite values with NaN. The function sets the plot style using Seaborn, then plots the closing price along with the moving average and Bollinger Bands. Additionally, it extracts and returns key financial figures, such as the latest price, beta, sector, country, and currency of the stock.

### Watchlist and Analysis
The script includes a predefined list of stock tickers to analyze. For each ticker in the watchlist, the script prints key financial figures and generates a stock price chart with indicators by calling the `plot_stock_with_indicators` function.

## Usage
To use the script, simply run it in a Python environment. It will iterate through the watchlist, generate plots, and print key financial figures for each stock.

## Example Output
For each stock in the watchlist, you will see a plot of the stock price along with the 20-day moving average and Bollinger Bands. Below the plot, the script will print key financial figures. For example, you might see details such as the latest price, beta, whether the stock is cyclical, its sector, country, and currency.

Feel free to reach out with any questions or suggestions!

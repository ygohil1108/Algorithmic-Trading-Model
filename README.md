# Algorithmic Trading Model

## Overview

This Python notebook contains an algorithmic trading model that utilizes various technical indicators to assess market volatility and track the general trend of SP500 stocks. The key indicators include Garman Klass Volatility, RSI (Relative Strength Index), Bollinger Bands, ATR (Average True Range), and MACD (Moving Average Convergence Divergence).

## Data Filtering and Clustering

- Filters SP500 stocks based on selected technical indicators.
- Implements a machine learning model to cluster stocks, with a focus on RSI.
- Selects stocks corresponding to the chosen cluster (e.g., Cluster 3).

## Portfolio Optimization

- Defines a function using the PyPortfolioOpt package and EfficientFrontier optimizer to optimize portfolio weights.
- Utilizes the last 1-year prices to optimize the weights.
- Applies single-stock weight bounds constraint for diversification.

## Sentiment Analysis and Signal Generation

- Loads the Twitter sentiment dataset.
- Sets the index, calculates engagement ratio, and filters out stocks with no significant Twitter activity.
- Calculates the prediction premium and its 6-month rolling standard deviation.
- Generates daily signals based on sentiment analysis.

## Execution Steps

To replicate the strategy, follow these steps:

1. **Data Preparation**
   - Ensure you have the necessary Python libraries installed (e.g., PyPortfolioOpt).
   - Load the SP500 stock data and technical indicators.
   - Execute the machine learning model for clustering.

2. **Portfolio Optimization**
   - Run the portfolio optimization function with the last 1-year prices.
   - Apply weight bounds for diversification.

3. **Sentiment Analysis**
   - Load the Twitter sentiment dataset.
   - Calculate engagement ratio and filter out stocks with minimal Twitter activity.
   - Compute the prediction premium and its rolling standard deviation.

4. **Signal Generation**
   - Generate daily signals based on sentiment analysis results.

## Note

This is the initial version of the trading strategy, and further improvements are envisioned, including incorporating real-time data and developing an application for portfolio optimization on platforms like Yahoo Finance.

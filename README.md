# Investing Strategy Based on Sentiment Analysis of Tweets in X

This repository contains a Jupyter Notebook that outlines an innovative investing strategy based on the sentiment analysis of Tweets related to stocks listed on the X market. The strategy leverages data-driven insights to select stocks monthly, based on their social media engagement and sentiment scores, and compares the performance with the NASDAQ index.

## Installation and Requirements

Before running the notebook, ensure you have the following software and packages installed:

- Python 3.11.6
- numpy 1.26.4
- pandas 2.2.2
- matplotlib 3.8.4
- yfinance 0.2.40

## Project Workflow

### Data Loading and Preprocessing
- Importing Data: Load the sentiment dataset, establish an index.
- Data Cleaning: Compute engagement ratios and filter out stocks with low activity on Tweets to focus on those with significant social media interactions.

### Monthly Aggregation
- Sentiment Analysis: Aggregate sentiment data monthly by each stock symbol and compute the average engagement ratio.
- Ranking: Calculate and rank stocks based on their monthly engagement ratio to identify top performers.

### Monthly Selection of Top 5 Stocks
- Stock Selection: At the start of each month, select the top five stocks based on the previous month's cross-sectional rankings.

### Portfolio Formulation
- Portfolio Setup: Create a dictionary mapping the start of each month to the stocks selected for the portfolio, ensuring timely updates and adjustments.

### Portfolio Performance Calculation
- Returns Calculation: Download and update stock prices monthly for the selected stocks to calculate and rebalance portfolio returns.

### Benchmark Comparison
- NASDAQ Benchmarking: Download the latest NASDAQ prices and calculate their returns to evaluate and compare with our strategy's performance.

## Usage
- To replicate the analysis or adapt it to your needs:

  - Ensure all dependencies are installed.
  - Run the Jupyter Notebook `SentimentInvestingStrategy.ipynb` to execute the code and view the analysis.

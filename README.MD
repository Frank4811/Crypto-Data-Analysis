# CoinMarketCap API Cryptocurrency Data Analysis

## Project Overview
This project uses the CoinMarketCap API to collect, analyze, and visualize cryptocurrency market data. It fetches the latest listings for top cryptocurrencies, including price changes over various time intervals, and tracks these trends over time.

## Features
- Retrieves real-time data for the top 15 cryptocurrencies by market cap using the CoinMarketCap Pro API.
- Cleans and normalizes JSON data into a Pandas DataFrame.
- Continuously appends data in timed intervals (every minute) to track historical changes.
- Handles API connection errors and rate limits gracefully.
- Provides exploratory data analysis including:
  - Average percentage price changes over multiple timeframes (1h, 24h, 7d, 30d, 60d, 90d).
  - Visualization of cryptocurrency price trends over time (example: Bitcoin).
- Outputs data both as DataFrames and CSV files for further analysis.

## Setup Instructions
1. Install required Python packages:
   ```bash
   pip install requests pandas seaborn matplotlib

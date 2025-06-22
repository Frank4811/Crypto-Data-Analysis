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
  - Visualization of cryptocurrency price trends over time (e.g., Bitcoin).
- Outputs data both as DataFrames and CSV files for further analysis.

## Setup Instructions
1. Install required Python packages:
   pip install requests pandas seaborn matplotlib

2. Obtain a CoinMarketCap Pro API key and replace it in the script:
   headers = {
       'Accepts': 'application/json',
       'X-CMC_PRO_API_KEY': 'YOUR_API_KEY_HERE',
   }

3. Run the script in a Jupyter notebook or Python environment.

4. If you're using Jupyter Notebook and encounter data rate limit issues, increase the limit with:
   jupyter notebook --NotebookApp.iopub_data_rate_limit=1e10

## Data Visualization
- Uses Seaborn and Matplotlib for plotting trends and point plots.
- Visualizes percentage changes across different time frames.
- Includes a line plot showing Bitcoin’s price trends over time.

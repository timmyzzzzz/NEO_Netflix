# Analyzing Netflix Historical Stock Prices - Data Visualization Portfolio Project

## Project Overview: 
This project focuses on using Python to explore and analyze the historical prices of Netflix stock, with the goal of using visualizations to answer the following questions:

- What has been the general trend of Netflix's stock price? 
- How can we visualize the price volatility to gain insight into expected fluctuations?
- How often did Netflix exceed their EPS (earnings per share) estimates when they reported earnings?
- Were there any trends between the movement of Netflix's stock price and any of the major US stock indices such as the Dow Jones Industrial Average, S&P 500 Index, or Nasdaq Composite?
- How can we identify potential trading opportunities by comparing the prices of Netflix's stock to its competitors, such as Disney and Spotify? 

The project code and results are contained in the Jupyter Notebook `analyze-netflix-stock.ipynb`, with a summary of the conclusions below.

Note that nothing in this project is intended as financial advice.

## Data: 
The `datasets` directory contains the historical daily and monthly OHLC stock prices for Netflix, major indices, and their competitors:
- `NFLX_daily_prices.csv` contains the daily OHLC stock prices for Netflix (`NFLX`) from 2020 to 2022
- `NFLX_monthly_prices.csv` contains the monthly OHLC stock prices for Netflix (`NFLX`) from 2020 to 2022
- Major indices include the Dow Jones Industrial Average (`DJI`), the S&P 500 index (`SP500`), and the Nasdaq Composite (`NASDAQ`)
- Competitors include Disney (`DIS`) and Spotify (`SPOT`)

The historical OHLC stock prices were scraped using the [yfinance](https://pypi.org/project/yfinance/) library. 

## Conclusion: 
In summary, this project provides valuable insights into the performance of Netflix stock from 2020 to 2022. Here are some key findings from the analysis:
- The distribution of daily percent returns looks relatively symmetric around the mean of about 0.044% and standard deviation of about 3.27%, which tells us that, on average, Netflix stock tended to gain value
- The outbreak of the COVID-19 pandemic and economic shutdowns resulted in the most volatile month (March 2020) for Netflix during this period
- Netflix has beaten EPS estimates in the last 5 quarterly earning reports (Q4-2021 to Q4-2022) which could be a sign that their stock price will rebound in the future
- The movement of Netflix stock is generally similar to the three major indices, though it seems to be more correlated to the Nasdaq Composite which makes sense since it is a more tech-heavy index
- Multiple mean reversions occurred in the price ratio of Netflix stock to its competitors Disney and Spotify in periods where the current price ratio was +/- 1 standard deviations from the historical mean price ratio

## Python Version and Library Dependencies
- Python (3.8.10)
- matplotlib==3.7.0
- numpy==1.22.2
- pandas==1.4.1
- seaborn==0.11.2

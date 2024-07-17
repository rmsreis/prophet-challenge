Copy code
# MercadoLibre Search Trends and Stock Price Analysis

## Project Overview

This project analyzes the relationship between Google search traffic for MercadoLibre and its stock price. The analysis aims to determine if search traffic can predict stock trading behavior and if there are any seasonal patterns in search traffic. The project is divided into four main steps:

1. **Find Unusual Patterns in Hourly Google Search Traffic**
2. **Mine the Search Traffic Data for Seasonality**
3. **Relate the Search Traffic to Stock Price Patterns**
4. **Create a Time Series Model with Prophet**

## Data

The following datasets are used in the analysis:
- **Google Hourly Search Trends**: Contains hourly search data for MercadoLibre.
- **MercadoLibre Stock Price**: Contains historical stock price data for MercadoLibre.

## Analysis Steps

### Step 1: Find Unusual Patterns in Hourly Google Search Traffic

1. Read the search data into a DataFrame and slice the data to May 2020.
2. Visualize the search traffic for May 2020.
3. Calculate and compare the total search traffic for May 2020 with the monthly median traffic across all months.
4. Identify any unusual patterns and relate them to corporate financial events.

### Step 2: Mine the Search Traffic Data for Seasonality

1. Group the hourly search data to plot the average traffic by the hour of the day.
2. Group the hourly search data to plot the average traffic by the day of the week.
3. Group the hourly search data to plot the average traffic by the week of the year.
4. Identify seasonal patterns and trends in the search traffic data.

### Step 3: Relate the Search Traffic to Stock Price Patterns

1. Read and plot the stock price data.
2. Concatenate the stock price data with the search data into a single DataFrame.
3. Slice the data to the first half of 2020 and visualize the trends.
4. Create new columns: Lagged Search Trends, Stock Volatility, and Hourly Stock Return.
5. Construct a correlation table to identify relationships between lagged search traffic, stock volatility, and stock price returns.

### Step 4: Create a Time Series Model with Prophet

1. Set up the search data for a Prophet forecasting model.
2. Estimate the model and plot the forecast to analyze near-term popularity trends.
3. Plot the individual time series components to answer specific questions about daily, weekly, and yearly trends.

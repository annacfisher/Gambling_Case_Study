# DS4002_project2
Project 2 github repository for DS 4002 group 16

## Contents
Time series analysis of DraftKing's adjusted stock price over the time period of April 2020 to January 2025. Analyzes the impact of major sporting events on adjusted stock price and builds a model using seasonality to predict future stock prices.

## Software and Platform

This project was conducted using Google Colab, R, and Python, utilizing pandas for data handling, matplotlib and seaborn for visualization, and various statsmodels for time-series analysis. Stock data was sourced via the Yahoo Finance API using the quantmod package in R. The project was executed on Mac and Windows platforms. The packages used in python were seaborn, pandas, matplotlib.pyplot, and numpy. Packages used in R to build our mdoel were dyplr, lubridate, tseries, and forecast.

## Map

### DATA folder:
- Data_Appendix.pdf
- dkng_ts.csv: raw data pulled from Yahood Finance
- weekly_dkng.csv: cleaned data used for analysis
### OUTPUT folder:
- EDA_Plots.md: EDA plots created
- Time_Series_Plots: Time series plots along with major sporting events
- Model_Prediction: Results of the model to predicting future DKNG stock price
### SCRIPTS folder
- 1_Data_Extraction.Rmd: Extracting DKNG stock data from Yahoo finance and cleaning for analysis
- 2_EDA_Scripts: Scripts used to explore trends, seasonality, and volatility in DraftKings stock data through time series, trading volume, decomposition, and differencing plots.
- 3_Sporting_Events_Analysis.ipynb: Time series plots looking at affect of major sports events on adjusted stock price
- 4_Seasonal_Model.Rmd: Building seasonal model in R and testing accuracy of predictions
### LICENSE
- MIT License dictating how this data and analysis can be used.

## Reproducing Results
To reproduce results, first use the 1_Data_Extraction.Rmd file to extract data from Yahoo finance. Use the commented out code to write a csv of the raw data. Use the code within the file to create a weekly time series of adjusted stock price to be analyzed, and save this as a seperate csv. Load the raw data into the 2_EDA_Scripts to see trends within the data. Open the 3_Sporting_Events_Analysis file and create time series graphs with shaded areas showing major sporting events. Lastly, use the 4_Seasonal_Model file with the weekly_dkng.csv data to build a seasonal model, predict future stock prices, and validate the model.

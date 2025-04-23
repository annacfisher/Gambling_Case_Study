# Gambling_Case_Study
GitHub repo for Betting Against Sports Betting Case Study - CS3 DS4002

## Contents
Case study analysis of DraftKings stock price. Students will analyze DraftKings stock over time and predict the next year of DraftKings prices to decide the optimal time to buy and sell the stock. The goal of the study is to figure out how to make the most money off of DraftKings's stock to win a bet against a friend.

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

## Results
This case study produced a predictive model with a mean average percent error of only 5%. However, the seasonal component of the model was not significant suggesting that seasonality surrounding sports does not produce stronger predictions. The model forecasts that DraftKings stock will continue to increase over the next year, so the optimal time to buy the stock is now. Previous years have shown a slight increase in stock price during March Madness, so the study suggests that buying the stock now and selling during March Madness will produce the greatest profits and help win the bet.

## Reproducing Results
To reproduce results, first use the 1_Data_Extraction.Rmd file to extract data from Yahoo finance. Use the commented out code to write a csv of the raw data. Use the code within the file to create a weekly time series of adjusted stock price to be analyzed, and save this as a seperate csv. Load the raw data into the 2_EDA_Scripts to see trends within the data. Open the 3_Sporting_Events_Analysis file and create time series graphs with shaded areas showing major sporting events. Lastly, use the 4_Seasonal_Model file with the weekly_dkng.csv data to build a seasonal model, predict future stock prices, and validate the model.

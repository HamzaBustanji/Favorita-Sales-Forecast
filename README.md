# Favorita-Sales-Forecast

<img src="https://github.com/HamzaBustanji/Favorita-Sales-Forecast/blob/main/images/download%20(1).svg"  width='60%' height='60%' align="right">

## Data 
The Data was provided in this [Kaggle competition.](https://www.kaggle.com/competitions/store-sales-time-series-forecasting/data)

## Summary
The aim of this project was to provide the giant Ecuadorian retailer, Favorita, with accurate monthly forecasts for the next quarter.
The steps we took to accomplish this task were: 

### Data Wrangling [[notebook]](https://github.com/HamzaBustanji/Favorita-Sales-Forecast/blob/main/notebooks/1-data-wrangling.ipynb)
* We loaded our data and displayed it
* We investigated missing values 
* We aggregated sales daily, monthly, and quarterly then we saved them for use in analysis and modeling
* We downloaded inflation data on Ecuador from the World Bank website, cleaned it, and saved it for later use

### Exploratory Data Analysis [[notebook]](https://github.com/HamzaBustanji/Favorita-Sales-Forecast/blob/main/notebooks/2-exploratory-data-analysis.ipynb)
* We investigated the effects of an earthquake that hit Ecuador in April of 2016 on aggregated sales
* We investigated the relationship between oil prices and sales. We calculated the correlation, super-imposed the two plots, and plotted a scatter plot
* We plotted holidays
* We looked into which stores had the highest sales, then used color to visualize whether the region the store is in played a role as well
* We investigated the seasonality and the trend in sales

<img src="https://github.com/HamzaBustanji/Favorita-Sales-Forecast/blob/main/images/Screen%20Shot%202023-04-25%20at%2011.12.00%20AM.png"  width='60%' height='60%' align="right">

* We performed an ETS decomposition
* We produced lag plots and auto-correlation plots 
* We visualized inflation, adjusted the sales for inflation, and plotted regular sales and inflation-adjusted sales
* We performed a Dickie-Fuller stationarity test



### Preprocessing and Modeling [[notebook]](https://github.com/HamzaBustanji/Favorita-Sales-Forecast/blob/main/notebooks/3-preprocessing-and-modeling.ipynb)
* We performed a train/test split
* We used AutoARIMA to find the best parameters of an ARIMA model and a SARIMA model
* We fit a Prophet model as well 
* We forecasted sales for the next quarter using these three models 
* We plotted the forecasted results against actual sales 
* We evaluated each model using the RMSE (Root Mean Square Error) metric 

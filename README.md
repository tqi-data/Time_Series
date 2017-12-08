# Time_Series

Insight time series tutorial: The goal of this notebook is introduce some key concepts for getting started with time series analysis. 

The data we will work with in this tutorial is real measurements of Antarctic Ice extent. As you can imagine, there is probably a strong seasonal aspect to ice melting and re-freezing, as well as possible long term climate change trends. The original data were on a daily timescale, but we will average within months to simplify things a bit.

For almost all time series analyses we are going to want to apply (at least some) statistical tests before we dive into modeling. Therefore, the first thing to do when working with time series data is to assess whether it is stationary.


This notebook is geared toward introducing core concepts of time series analytics. There are a few key take aways:

Stationarity is an important assumption when decomposing time series data and should be the first thing you assess
       The Augmented-Dickey Fuller test is useful to test if a time series is stationary
        You can always transform your data to make it stationary: de-meaning, differencing, and decomposing are common methods
Examining trend and seasonal components are great ways to understand the behavior of a time series
        Trend may tell you long term patterns such as decreasing ice extent over a period of decades
              Trend can be estimated with rolling means or decomposition
        Seasonality is helpful for understanding short term behaviors
              You can observe seasonality by removing trend, or through decomposition
Granger Causality is useful for testing the relationship of two time series
        Keep in mind the caveat that it is possible to have bi-directional Granger Causality

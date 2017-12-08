# Time_Series

Insight time series tutorial: The goal of this notebook is introduce some key concepts for getting started with time series analysis. 

The data we will work with in this tutorial is real measurements of Antarctic Ice extent. As you can imagine, there is probably a strong seasonal aspect to ice melting and re-freezing, as well as possible long term climate change trends. The original data were on a daily timescale, but we will average within months to simplify things a bit.

For almost all time series analyses we are going to want to apply (at least some) statistical tests before we dive into modeling. Therefore, the first thing to do when working with time series data is to assess whether it is stationary.

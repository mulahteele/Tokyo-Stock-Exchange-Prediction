
# Autoregressive Integrated Moving Average(ARIMA)

## Definition

An autoregressive integrated moving average, or ARIMA, is a statistical analysis model that uses time series data to either better understand the data set or to predict future trends(which are often interpreted similarly to that of a multiple linear regression model).

A statistical model is autoregressive if it predicts future values based on past values. For example, an ARIMA model might seek to predict a stock's future prices based on its past performance or forecast a company's earnings based on past periods.

-**Autoregression (AR):** refers to a model that shows a changing variable that regresses on its own lagged, or prior, values.(The predicted value)


-**Integrated (I):** represents the differencing of raw observations to allow the time series to become stationary (i.e., data values are replaced by the difference between the data values and the previous values).(More differentiation to make the data more stationary in order to feed into the model)

**why:** A model that shows stationarity is one that shows there is constancy to the data over time. Most economic and market data show trends, so the purpose of differencing is to remove any trends or seasonal structures. Seasonality, or when data show regular and predictable patterns that repeat over a calendar year, could negatively affect the regression model. If a trend appears and stationarity is not evident, many of the computations throughout the process cannot be made and produce the intended results.


-**Moving average (MA):**  incorporates the dependency between an observation and a residual error from a moving average model applied to lagged observations.(The bias)


## Parameters

**p:** the number of lag observations in the model, also known as the lag order.

**d:** the number of times the raw observations are differenced; also known as the degree of differencing.

**q:** the size of the moving average window, also known as the order of the moving average.

## Pros                                                           Cons
- Good for short-term forecasting                                  - Not built for long-term forecasting

- Only needs historical data                                       - Poor at predicting turning points

- Models non-stationary data                                       - Computationally expensive

                                                                   - Parameters are subjective













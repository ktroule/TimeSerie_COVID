# Time series analysis
The objective is to gain understanding (the basics) of time series analyses to extrapolate/forecast future times.


### Components of time series
`time serie = signal + noise`

- Signal is composed of two components:
  - Seasons: repeated pattern every specifcic interval.
  - Trends/cycle: global patter (up/down) across seasons. Cycle refers to when trends do not repeat regulary.
- Noise also termed as error:
  - Noise: random noise/residual component.

### Stationarity of time series
It's the time series in which the average and variance remain constant so properties are *indepentent of time*.
- Time series with trends are **not** stationary.
- Data must be transform our time series to stationary before feeding it to statistcal models. If the values of the data (average, variance) change over time, it's hard for ml models to predict. **Thus, data must convert into non-stationary time series**.

### Convert non-stationary time series to stationary
A basic and common approach can be to take the difference (differentiating) between the values of adjacent time points.
This will lilekly correct the difference in the mean along the time period but might not correct the variance.
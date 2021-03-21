# Power-Market_prediction
Predicting Spanish Electricity Prices

The goal of this assignment is to build a Machine Learning model to predict the electricity prices in Spanish Market. 
The Power-Market.csv will be our train set and scoring will be the data on which we will do the prediction.

The power market is like many markets in which the price is settled where demand meets supply.

•Supply: power generation plants (nuclear, solar, wind, etc).  Each type of production is different and should be analyzed independently before making assumptions.  Analyzing seasonality, distributions and correlations is advised.

•Demand: all the power consumption in the country, from huge factories to small house-hold consumers.  Very seasonal and heavily affected by temperature.The data provided is of timeseries form, meaning you should be careful when splitting for train and test.

The provided datasets contain the following timeseries with hourly granularity:

•date:  date of the observation ”%Y-%m-%d”

•hour:  hour of the observation, [0 - 23]

•fcdemand:  forecast of demand in MWh

•fcnuclear:  forecast of nuclear power production in MWh

•importFR: forecast of the importing capacity from France to Spain in MWh

•exportFR: forecast of the exporting capacity from Spain to France in MWh

•fcwind:  forecast of wind power production in MWh

•fcsolarpv:  forecast of PV solar (solar panels) power production in MWh

•fcsolarth:  forecast of thermal solar power production in MWh

•price:  power price for each hour in€/MWh.This is the target we want to predict.


Information from Portfolio Management

•The price of the power market is heavily affected by demand and also by those powerproducers with higher costs of production like coal, gas, etc.  Those forecasts are notavailable, but you can infer how much ”expensive production” is needed by substractingto the demand the energy provided by nuclear, wind and solar.  This is called ThermalGap

•Analyze each timeseries by itself:  look for outliers, NaNs, and see their distributions.Look for skewed distributions and think if you can convert the values into categories•When dealing with feature engineering, a good start point can be checking the differ-ences, ratios, absolute differences between demand and each power production time-series.

•Create new features out of what we already know like the seasonality of solar production and the different periods of the day.  Think that demand is heavily affected byhuman behavior and human behavior heavily depends on the sun!

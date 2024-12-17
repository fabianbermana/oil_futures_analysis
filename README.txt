### Introduction ###
This is a personal project to investigate the relationships present within and between the three main oil futures used as global benchmarks: Brent, WTI, and Dubai. The data is obtained from: https://uk.investing.com/commodities/crude-oil-historical-data

One issue with the data is that the Dubai futures are only available from 2014, while we are able to retrieve Brent and WTI futures data from significantly further history. To let us investigate potential correlations and cointegrations between the three time series, for this project, we discard any dates where not all of the three prices are available, and will continue to do so until a more complete data source is found.

### Contents ###
The aim is to apply both 'classical' statistical and econometric methods, such as ARMA and GARCH models, and machine learning models such as recurrent neural networks. The former has the advantage of being easily interpretable, while the latter aims to produce more accurate predictions and find non-linear relations within datasets.

Currently, the repository contains the following items:

(Folder) Datasets:
    Contains the historical data of oil futures.

(Folder) scripts:
    Contains ipython notebooks used to run our analysis.

    - data_cleaning.ipynb: Notebook used to combine the three oil futures together into a single .csv file.
    - exploratory_analysis.ipynb: Notebook with simple plots and visualizations of our data.
    - time_series_analysis_basic.ipynb: Notebook with ARMA models and basic statistical tests.

We plan to add:

- time_series_analysis_intermediate.ipynb: Notebook containing more advanced time series models, such as GARCH for stochastic volatility, VAR, and VECM.
- machine_learning_models.ipynb: Notebook containing machine learning predictors of the oil returns.

# EU Electricity Market Time Series Analysis

This project was done as my first year Masters thesis at the Toulouse School of Economics. It is an extension of a previous project I did in collaboration with Moongyeom Kim for an Applied Econometrics project. That original project can be found [here](https://github.com/aboomer07/EuropeEnergyPanel).

## Overview
The original project used a panel approach to analyze the effect of renewable electricity penetration on balancing market outcomes in 20 EU member states. Given the nature of high frequency electricity data, persistent serial autocorrelation was found in the residuals. This thesis project investigated using a time series treatment of the model as opposed to the original panel model. To this end, a bayesian structural time series (bsts) model with markov chain monte carlo (MCMC) based estimation was used. The paper also looks at the historical progression of time series modeling, and how different time series behavior is captured in different models. Data was additionally analyzed in the frequency space using the Fourier transform to gain insight into cyclical patterns.

## Data Sources
The data is sourced from the European Network of Transmission System Operators for Electricity (ENTSO-e) transparency database. The data is downloaded with a HTTP based API, which returns XML files containing the data. The database can be found [here](https://transparency.entsoe.eu).

## Tools
The paper was built using Latex. The coding was done in R using the bsts, tidyverse, XML, stringr, plm, stargazer, sandwich, stats, forecast, and tseries packages.

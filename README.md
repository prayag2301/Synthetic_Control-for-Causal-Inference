# Synthetic Control for Causal Inference
## Introduction and Background
The Paris Agreement (2015) emphasized the common goal of mitigating global warming.
Public support for a carbon tax is low and actual implementation and empirical studies on their effects are limited.
This quasi-experimental study seeks to address the gap by finding a significant causal effect of carbon taxes on emissions in the case of Sweden.

### Why Sweden?
Sweden was one of the first countries in the world to implement a carbon tax in 1991.
Less vulnerable to carbon leakage from the transportation sector, hence emission reductions are unbiased.
Able to capture adjustments made on both intensive and extensive margins.
#### This study investigates the effects of Sweden environmental tax reform during 1990-1991 on per capita CO2 emissions. Annual panel data from transport on CO2  emissions are collected for 25 OECD countries, focusing on the period between 1960 and 2005

## SCM Model Description
Construct a counterfactual, “synthetic Sweden”: consisting of a weighted combination of countries that did not implement carbon taxes or similar policies during the treatment period and that before treatment resemble Sweden on several key predictors of CO2 emissions.

* Treated unit: Sweden Control: 14 OECD countries
* Pre-treatment period: 1960-1989 Post-treatment period: 1990-2005
* Key predictors: GDP per capita, number of motor vehicles, gasoline consumption/capita, percentage of urban population and 3 lagged years of CO2 emissions 1970, 1980, 1989
* Outcome variable: metric tons of CO2 per capita

  | Weights |    Countries      |
  | --------|------------------ |
  | 0.381   |       Denmark     |
  | 0.199   |       Belgium     |
  | 0.175   |       New Zealand |
  | 0.090   |        Greece     |
  | 0.089   |      United States|
  | 0.063   |       Switzerland |
  | 0.002   |        Poland     |
  | 0       | Australia, Canada,|
  |         | France, Finland,  |
  |         |  Japan, Spain,    |
  |         |  Portugal         |
  |         |                   |

## Results
#### Synthetic Control Method confirms Sweden's carbon tax significantly and credibly reduced CO2 emissions

### Emission Reduction
Emissions declined by 11% relative to a synthetic control unit composed of OECD countries that did not implement similar policies
### Placebo Test Validity
In-time and in-space placebo tests revealed no significant placebo effects, confirming the impact of the carbon tax on reducing CO2 emissions
The leave-one-out test demonstrated robust results, further confirming the effectiveness of the carbon tax in reducing emissions

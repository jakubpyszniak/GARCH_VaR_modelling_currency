# VaR analysis of EUR/PLN

We estimate several GARCH-type models (GARCH, EGARCH, AR-GARCH, GARCH-in-mean, GARCH-t) in order to predict yearly $ VaR_{0.05\%} $ and $ VaR_{99.5\%} $. We check different quantiles as a decrease or increase of an exchange rate influences assets and liabilities. It is not generally clear whether the cumulative effect is positive or negative - monitoring both allows a firm to check which effect is greater in a real scenario.

# Structure

The entire analysis is contained in a single finished notebook. Our full analysis covers:

* EDA for the EUR/PLN exchange rate (log returns)
* Checking for GARCH effects (volatility clusters, leverage effects, leptokurtosis, Engle test)
* Training of different models (removing autocorrelation, explaining the advantages of model specifications)
* Daily $ VaR_{0.05\%} $ and $ VaR_{99.5\%} $ prediction and assessment based on the number of exceedances (in-sample and out-of-sample)
* Model selection based on the least number of out-of-sample exceedances
* Yearly $ VaR_{0.05\%} $ and $ VaR_{99.5\%} $ prediction utilising additive log returns and Monte Carlo simulations.
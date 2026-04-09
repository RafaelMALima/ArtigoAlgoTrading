# Statistical Arbitrage Between Cointegrated Equities and Commodity Futures

This repository contains the research notebook and conference-style paper for a statistical arbitrage study that tests whether commodity-producing companies can be paired with futures on their underlying commodities.

The project evaluates candidate stock–futures pairs across three sectors:

- **Oil & energy**
- **Mining / iron ore**
- **Livestock / food production**

Using daily data, the workflow first screens pairs with the **Engle–Granger cointegration test** on a 2015–2019 in-sample window, then runs an out-of-sample **pairs trading backtest** over 2020–2025 with a rolling hedge ratio, z-score entry/exit rules, position caps, and idle cash remunerated at the CDI benchmark. According to the paper, the most promising pairs were **Chevron (CVX) vs. crude oil futures (CL=F)** and **BHP vs. iron ore futures (TIO=F)**, while the livestock-related pairs did not show useful evidence of cointegration.

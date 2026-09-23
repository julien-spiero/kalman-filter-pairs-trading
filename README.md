# Kalman Filter Pairs Trading Strategy

A quantitative research project exploring **intraday statistical arbitrage** using a dynamic hedge ratio estimated with a **Kalman Filter**.

## Overview

The strategy identifies cointegrated pairs of futures and dynamically estimates their hedge ratio using a Kalman Filter, rather than relying on a static OLS regression.

The strategy was tested on **hourly Copper and Silver futures data**, using z-score based entry and exit signals while accounting for transaction costs and slippage.

## Methodology

* **Pair selection:** Engle-Granger cointegration test
* **Hedge ratio:** Dynamic estimation with Kalman Filter
* **Signal:** Spread z-score
* **Frequency:** Hourly
* **Backtesting:** Transaction costs, slippage and no look-ahead bias
* **Benchmark:** Static OLS hedge ratio

## Results

For the Copper/Silver pair:

* **Sharpe Ratio:** 0.37
* **Hit Ratio:** 67%

## Tech Stack

Python · Pandas · NumPy · Statsmodels · PyKalman · Matplotlib

## Repository Structure

```text
├── kalmanFilterStrategy.py
├── data/
├── data1/
└── README.md
```

## Disclaimer

This project is for research and educational purposes only and does not constitute investment advice.

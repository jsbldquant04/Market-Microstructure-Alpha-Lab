# Order Flow Imbalance & Short-Term Price Dynamics

An empirical quantitative research project investigating whether **order-flow imbalance** contains information about short-term cryptocurrency price movements.

The project uses real BTCUSDT trade-level data to construct order-flow features, analyze their relationship with future returns, and evaluate a simple research hypothesis using statistical analysis and out-of-sample testing.

## Research Question

> Does order-flow imbalance contain predictive information about short-term BTCUSDT returns?

The primary variable is:

$$
OFI_t =
\frac{V_{buy,t}-V_{sell,t}}
{V_{buy,t}+V_{sell,t}}
$$

where $\(V_{buy}\)$ and $\(V_{sell}\)$ represent aggressively executed buy and sell volume.

## Research Workflow

```text
Real Trade Data
      ↓
Data Cleaning
      ↓
Trade Classification
      ↓
Order-Flow Features
      ↓
Exploratory Analysis
      ↓
Hypothesis Testing
      ↓
Statistical Modeling
      ↓
Out-of-Sample Evaluation
      ↓
Transaction-Cost-Aware Backtest
      ↓
Research Conclusions
```

## Topics Covered

* Market microstructure
* Trade-level data
* Aggressive buying and selling
* Order-flow imbalance
* Short-term price dynamics
* Price impact
* Absorption
* Time-series analysis
* Statistical hypothesis testing
* Look-ahead bias
* Transaction costs
* Out-of-sample validation
* Quantitative research methodology

## Data

The project uses publicly available **BTCUSDT trade-level market data from Binance**.

The analysis aggregates individual executions into one-minute intervals to study the relationship between order flow and subsequent price returns.

## Key Research Questions

The notebook investigates:

1. Is order-flow imbalance associated with future returns?
2. Does extreme order flow behave differently from neutral flow?
3. Is the relationship statistically significant?
4. Does the relationship remain after accounting for transaction costs?
5. Does the observed relationship persist on unseen data?
6. Can additional microstructure features improve prediction?

## Project Scope

This repository is **research-oriented**.

It is intended to demonstrate a quantitative research workflow for investigating market microstructure phenomena. It is **not** intended to be a production-grade trading system, execution engine, or investment recommendation.

The purpose is to investigate a market hypothesis empirically and determine whether the observed relationship is supported by the data.

## Technologies

* Python
* Pandas
* NumPy
* SciPy
* Scikit-learn
* Matplotlib
* Seaborn
* Binance public market data API
* Google Colab

## Future Research

Possible extensions include:

* Level-2 order-book data
* Order-book imbalance
* Bid/ask spread dynamics
* Liquidity and market depth
* Price-impact modeling
* Cumulative Volume Delta
* Hawkes processes
* Regime-dependent order flow
* Market-impact models
* More rigorous walk-forward validation

## Disclaimer

This project is for **educational and research purposes only**. Statistical relationships observed in historical market data do not imply future profitability or investment performance.

# Order Flow Imbalance & Short-Term Price Dynamics

An empirical quantitative research project investigating whether **order-flow imbalance** contains information about short-term cryptocurrency price movements.

The project uses real BTCUSDT trade-level data to construct order-flow features, analyze their relationship with future returns, and evaluate a research hypothesis using statistical analysis and out-of-sample testing.

## Research Question

> Does order-flow imbalance contain predictive information about short-term BTCUSDT returns?

The primary variable is:

$$
OFI_t =
\frac{V_{buy,t}-V_{sell,t}}
{V_{buy,t}+V_{sell,t}}
$$

where $V_{buy}$ and $V_{sell}$ represent aggressively executed buy and sell volume.

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

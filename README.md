# Dynamic Alpha Scanner (V6)

### Quantifying Market Outperformance through Beta-Neutrality

The **Dynamic Alpha Scanner** is a quantitative trading tool developed in **Pine Script 6**. It solves the epistemological problem of nominal price movement by isolating an asset's idiosyncratic strength (**Alpha**) from its systematic market exposure (**Beta**).

In a world of high correlation, seeing a green candle is not enough. This scanner identifies if an asset is truly attracting capital or simply floating with the tide of the benchmark.

## Core Logic
- **Beta-Neutrality:** It calculates the rolling Beta using Pearson correlation and relative volatility.
- **Jensen's Alpha Isolation:** It subtracts the expected risk-adjusted return from the actual return.
- **Inertia Filtering:** Candles are colored based on the acceleration of Alpha, not just its polarity.

## Visual Indicators
- **Green (Outperforming):** Positive Alpha with increasing momentum.
- **Red (Underperforming):** Negative Alpha with decreasing momentum.
- **Gray (Neutral):** Mean reversion or loss of relative strength.

# Technical Methodology: The Math Behind the Alpha

### 1. The Nominal Price Fallacy
Price in isolation is a noisy signal. For a trader, the only thing that matters is the **Relative Strength Index (RS)** adjusted for risk. 

### 2. The Alpha Formula
We utilize a simplified version of Jensen's Alpha for real-time series analysis:
$$Alpha = R_i - \beta \cdot R_m$$
Where:
- $R_i$: Return of the Asset (Rate of Change)
- $R_m$: Return of the Benchmark (Market)
- $\beta$: The asset's sensitivity to the market.

### 3. Beta Calculation
Instead of a static Beta, we use a rolling window of 20 periods:
$$\beta = \rho_{im} \cdot \left(\frac{\sigma_i}{\sigma_m}\right)$$
This ensures the scanner adapts to changing market regimes (low vs. high volatility).

### 4. Inertia & Momentum
To avoid "whipsaws", we apply an Exponential Moving Average (EMA) to the Alpha signal. A color change only triggers if the Alpha is both above/below zero AND moving in the direction of the divergence ($ta.rising$ or $ta.falling$).

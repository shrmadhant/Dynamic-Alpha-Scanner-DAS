# Trading Strategies with Alpha Scanner

### 1. The Convergence Setup (Trend Following)
- **Market Condition:** Benchmark is in a clear trend.
- **Signal:** Asset candles turn Green.
- **Logic:** The asset is gaining more value than the index itself, indicating institutional "heavy lifting".

### 2. The Divergence Setup (Mean Reversion)
- **Price:** Making new lows.
- **Alpha Scanner:** Turning Gray or Green.
- **Logic:** Absorption. The market is falling, but the asset has stopped underperforming. This is a primary signal for a potential bottom.

### 3. The "Dead Weight" Exit
- **Price:** Rising.
- **Alpha Scanner:** Turning Red.
- **Logic:** The asset is rising only because the Beta is high, but it's losing Alpha. Exit the position before the benchmark corrects, as this asset will likely fall harder.

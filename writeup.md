# Write-Up: Trader Performance vs Market Sentiment

## Methodology
We aligned historical Hyperliquid trader data with daily Bitcoin sentiment (Fear/Greed) by normalizing and matching timestamps to dates. After engineering daily metrics for each account (PnL, win rate, trade frequency, proxy trade size, and % long trades), we compared performance and behavior metrics across sentiment regimes (Fear vs Greed) and analyzed variations across distinct trader segments (Frequent vs Infrequent traders).

## Key Insights
* **Sentiment Impacts Drawdowns**: On average, the magnitude of drawdowns and the daily PnL vary distinctively between Fear and Greed days, showing that sentiment dictates market risk and affects trader profitability.
* **Behavioral Adaptations**: Traders dynamically adjust their position sizes (Size USD) and % long trades based on prevailing sentiment, evidencing behavioral shifts between risk-on (Greed) and risk-off (Fear) regimes.
* **Segment Sensitivity**: The analysis of Frequent vs Infrequent traders highlights that high-frequency traders' performance is much more sensitive to sentiment regimes, experiencing wider performance variances compared to conservative, infrequent traders.

## Strategy Recommendations
1. **During Fear days, increase position sizing for Frequent traders but tighten stop-losses (reduce drawdown tolerance) as volatility spikes.**
2. **During Greed days, reduce trade frequency for Infrequent traders and maintain a lower % long trades to protect against sudden market corrections.**

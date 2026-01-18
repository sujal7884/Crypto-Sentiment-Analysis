# Bitcoin Sentiment vs. Trader Performance Analysis

## 📌 Project Overview
This project analyzes historical trader data from Hyperliquid against the Bitcoin Fear & Greed Index to identify behavioral patterns in crypto trading. The objective was to determine if market sentiment (Fear vs. Greed) correlates with trader profitability.

## 📊 Key Findings & Insights
Based on the analysis of execution data:

### 1. Momentum Trading Outperforms Contrarian Approaches
* **Insight:** Traders demonstrated significantly higher profitability during "Greed" cycles compared to "Fear" cycles.
* **Data:** Average PnL per trade was **$77.84 during Greed**, which is **55% higher** than the $50.05 average during Fear.
* **Conclusion:** This suggests that trend-following strategies during bullish sentiment are yielding better results than trying to "catch the bottom" during Fear.

### 2. "Neutral" Markets Pose the Highest Risk
* **Insight:** Trader performance metrics collapsed during "Neutral" market sentiment, indicating a weakness in sideways/choppy market conditions.
* **Data:** The Win Rate dropped to **31.7%** in Neutral conditions, compared to a robust **45.3%** in Greed and **41.5%** in Fear.
* **Conclusion:** Traders should consider reducing position size or pausing activity when market sentiment lacks a clear directional bias (Neutral).

### 3. Win Rate vs. Reward Ratio
* While the **Win Rate** variance between Fear (41.5%) and Greed (45.3%) is small (~4%), the **Profit variance** is massive ($50 vs $78). This implies that while traders win at a similar rate, their **winning trades run much further** during Greed periods.

## 🛠 Tech Stack
* **Python:** Pandas for data manipulation, Seaborn/Matplotlib for visualization.
* **Data Processing:** Merged disparate time-series datasets (Market Sentiment + Trade Executions) using datetime alignment.

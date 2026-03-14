# trader-sentiment-analysis
Trader behavior analysis using Bitcoin Fear &amp; Greed sentiment and Hyperliquid trading data
# Trader Behavior vs Market Sentiment Analysis

## Overview

This project analyzes how Bitcoin market sentiment (Fear vs Greed) influences trader behavior and trading performance on the Hyperliquid platform.

By combining historical trading data with the Bitcoin Fear & Greed Index, this analysis identifies behavioral patterns among traders and proposes actionable trading strategies based on sentiment regimes.

The goal is to uncover insights that can help traders adjust their strategies depending on prevailing market sentiment.

---

## Problem Statement

Market sentiment is known to influence trading decisions and market dynamics.  
This project investigates how trader performance and behavior change across different sentiment regimes.

Key questions addressed:

1. Does trader performance (PnL, win rate) differ between Fear and Greed market conditions?
2. Do traders change behavior depending on sentiment (trade frequency, trade size, position direction)?
3. Can traders be segmented into behavioral groups such as frequent vs infrequent traders?
4. What actionable trading strategies can be derived from these insights?

---

## Datasets

### 1. Bitcoin Market Sentiment Dataset
This dataset contains the Bitcoin Fear & Greed Index, which measures market sentiment daily.

Columns include:
- timestamp
- classification (Fear, Greed, Extreme Fear, Extreme Greed, Neutral)
- sentiment value
- date

### 2. Hyperliquid Historical Trader Dataset
This dataset contains trade-level data for traders on the Hyperliquid platform.

Columns include:
- Account
- Coin
- Execution Price
- Size USD
- Side
- Closed PnL
- Timestamp IST

---

## Methodology

The analysis follows these steps:

1. Data Loading and Exploration
2. Data Cleaning and Preparation
3. Timestamp Conversion and Date Alignment
4. Merging Trader Data with Sentiment Data
5. Feature Engineering
6. Behavioral Analysis
7. Trader Segmentation
8. Strategy Recommendations

---

## Feature Engineering

Additional metrics were created to analyze trader behavior:

- Daily PnL per trader
- Win indicator for profitable trades
- Trade frequency
- Average trade size
- Trader segmentation (frequent vs infrequent traders)

---

## Key Insights

1. **Trading Activity Increases During Greed**
   - Traders are significantly more active when market sentiment is positive.

2. **Trade Sizes Increase in Greed Markets**
   - Traders take larger positions when confidence in the market is high.

3. **Fear Markets Show Higher Risk**
   - Profit/loss distributions during Fear periods are more volatile.

4. **Trader Behavior Changes With Sentiment**
   - Long positions are more common during Greed markets, indicating bullish expectations.

---

## Strategy Recommendations

### Strategy Rule 1: Reduce Risk During Fear Markets
During Fear or Extreme Fear sentiment regimes, traders should reduce position sizes and limit trading frequency due to increased volatility and downside risk.

### Strategy Rule 2: Utilize Momentum During Greed Markets
During Greed periods, traders may benefit from momentum-based strategies such as trend-following and increased trading activity, while maintaining proper risk management.

---

## Tools & Libraries

The project was implemented using:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn (for optional clustering analysis)

---

## Project Structure
Trader-Sentiment-Analysis/
│
├── analysis.ipynb
├── README.md
├── charts/
└── data/

## Conclusion

This analysis demonstrates that market sentiment plays an important role in shaping trader behavior and performance.

By integrating sentiment indicators with trading data, traders can adjust strategies based on prevailing market psychology and improve risk management.

---

## Author

Hemavathi Nandhakumar

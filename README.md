# Trader Behavior vs Market Sentiment Analysis

## Overview
This project analyzes how Bitcoin market sentiment (Fear and Greed Index) relates to trader behavior and performance on Hyperliquid. The objective is to uncover behavioral patterns and derive actionable trading insights.

## Dataset
- Bitcoin Fear and Greed Index (daily sentiment classification)
- Hyperliquid historical trader data (executions, pnl, leverage, etc.)

## Methodology

### Data Preparation
- Cleaned and validated both datasets
- Converted timestamps to daily level
- Merged trader activity with market sentiment
- Engineered key metrics such as daily PnL, win rate, trade frequency, and position size

### Analysis
- Compared trader performance across sentiment regimes
- Measured behavioral changes during Fear vs Greed
- Segmented traders by trading frequency
- Evaluated downside risk using negative day ratio

### Bonus Modeling
- Built a Random Forest model to predict next-day profitability using sentiment

## Key Insights
- Trader profitability and win rate are highest during Extreme Greed periods
- Trade activity increases significantly during Fear conditions
- Traders take larger position sizes during fearful markets
- Infrequent traders outperform frequent traders, indicating overtrading risk
- A simple predictive model using sentiment achieved about 60 percent accuracy, showing moderate predictive signal

## Strategy Recommendations
1. Maintain normal exposure during Extreme Greed but avoid excessive leverage
2. Reduce position size and leverage during Fear periods to control downside risk
3. Prefer selective trading over high-frequency trading

## How to Run
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook
```

Open the notebook and run all cells sequentially.

## Author
Gokul S

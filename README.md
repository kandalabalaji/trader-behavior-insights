# Trader Behavior & Market Sentiment Analysis

This project analyzes how trader performance and risk behavior change across market sentiment regimes using Hyperliquid historical trades and the Bitcoin Fear & Greed Index.

## Data
- historical_data.csv – trader level executions and PnL
- fear_greed_index.csv – daily sentiment (classification and score)

## Method
Trades are aligned to daily sentiment using timestamp-based joins, then aggregated per account and day to compute daily PnL, average trade size, trade count and buy ratio. Traders are segmented into Retail, Mid and Whale cohorts based on average trade size.

## Key Outputs
- Daily trader features by sentiment  
- Segment-wise performance comparison  
- Visualization of average daily PnL across sentiment regimes

## How to Run
Open the notebook in Google Colab, update the data paths, and run all cells top to bottom.

## Limitation
Only 77 daily records are usable because sentiment data does not fully overlap with the trading period.

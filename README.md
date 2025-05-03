# Trading Game

This project implements a systematic  strategies on different price data.

## Strategy 1 Overview

- **Strategy**: SMA Crossover (SMA 5 vs SMA 20)
- **Assets**: 9 Global Equity ETFs (SPY, QQQ, EWJ, ASHR, etc.)
- **Signals**: Long when SMA(5) crosses above SMA(20), Short when below
- **Data**: Weekly prices from 2010 to 2025
##  What Was Done - Stategy 1 

- Implemented three strategies: **SMA, Momentum, Reversal**
- Focused on SMA Crossover with trade signal generation
- Backtested all signals: calculated PnL, win rate, Sharpe ratios
- Filtered for **high-quality trades (PnL > 2%, Sharpe > 0.2)**
- Built **realistic trading logs**, including a recent signal from **April 2025**
- Exported logs in CSV format ready for submission or live simulation

##  Strategy 2: Gold vs BCOM Divergence

- **Hypothesis**: When gold price increases while BCOM Index (commodity benchmark) drops, gold may act as a safe-haven → signal to Long Gold
- **Data**: Daily Gold Futures and Bloomberg Commodity Index (2015–2025)
- **Signal**: Long Gold when gold return – BCOM return > threshold (e.g., 2–4%)
- 
### ✅ What Was Done - Stategy 2

- Built signal and divergence indicator
- Ran backtest with 5-day holding window
- Calculated PnL, win rate, Sharpe ratio
- Generated live trading log for April 2025


## Files Included

| File | Description |
|------|-------------|
| `Trading_game_strategies.ipynb` | Main Jupyter Notebook with all code and visualizations |
| `Spot ETFS for Major Global Indices.xlsx` | Historical ETF weekly prices |
| `signals_summary.csv` | All generated SMA crossover signals |
| `Trading_Log_2025-04-22.csv` | Trading log based on the latest valid signal (April 2025) |
| `Trading_Log_Ready.csv` | Filtered, high-confidence trades with comments |
| `Commodity_based_strategy.ipynb` | Gold vs BCOM divergence strategy notebook |
| `Trading_Log_Gold.csv` | Historical divergence signals and trades |
| `Trading_Log_Live_commodities.csv` | Real-time signal from April 2025 (LIVE log) |



##  Summary

Two quantitative strategies were developed and tested:
- The **ETF SMA crossover** showed consistent results and generated viable trades.
- The **Gold divergence model** was statistically weak, and the hypothesis was **rejected based on backtest performance**( what if we buy gold when it's rising and the entire commodity market is falling?- **rejected**)


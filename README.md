# Trading Game

This project implements a systematic SMA crossover strategy on weekly ETF price data.

## Strategy Overview

- **Strategy**: SMA Crossover (SMA 5 vs SMA 20)
- **Assets**: 9 Global Equity ETFs (SPY, QQQ, EWJ, ASHR, etc.)
- **Signals**: Long when SMA(5) crosses above SMA(20), Short when below
- **Data**: Weekly prices from 2010 to 2025

##  What Was Done

- Cleaned and structured historical ETF price data
- Implemented three strategies: **SMA, Momentum, Reversal**
- Focused on SMA Crossover with trade signal generation
- Backtested all signals: calculated PnL, win rate, Sharpe ratios
- Filtered for **high-quality trades (PnL > 2%, Sharpe > 0.2)**
- Built **realistic trading logs**, including a recent signal from **April 2025**
- Exported logs in CSV format ready for submission or live simulation

## Files Included

| File | Description |
|------|-------------|
| `Trading_game_strategies.ipynb` | Main Jupyter Notebook with all code and visualizations |
| `Spot ETFS for Major Global Indices.xlsx` | Historical ETF weekly prices |
| `signals_summary.csv` | All generated SMA crossover signals |
| `Trading_Log_2025-04-22.csv` | Trading log based on the latest valid signal (April 2025) |
| `Trading_Log_Ready.csv` | Filtered, high-confidence trades with comments |
| `README.md` | Project summary and file descriptions |

##  Key Insight

Only one valid SMA crossover signal  was found close to present time (April 2025), confirming how rare clean technical signals can be.


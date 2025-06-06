# Momentum Strategy Backtest (Alpha Signal)

This project builds and backtests a simple momentum-based long-only equity strategy.

## Strategy Overview

- **Universe**: FAANG stocks (FB, AAPL, AMZN, NFLX, GOOGL)
- **Signal**: 6-month price momentum = price(t) / price(t−126)
- **Portfolio**: Long top 3 ranked stocks, equal-weighted
- **Rebalancing**: Monthly
- **Benchmark**: S&P 500 (SPY)

## Skills Demonstrated

- Signal-based portfolio construction
- Backtesting logic using `pandas`
- Performance evaluation (cumulative returns, Sharpe ratio)
- Data visualization

## Sample Output

- 📈 Cumulative returns vs SPY
- 📊 Monthly portfolio composition
- 🔁 Signal evolution over time

## Future Improvements

- Include transaction costs
- Add risk management filters (e.g., volatility targeting)
- Compare with alternative signals (e.g., reversal, RSI)

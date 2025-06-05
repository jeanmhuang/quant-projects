# Portfolio Optimization: Efficient Frontier (AAPL, MSFT, GOOGL)

This project uses Monte Carlo simulation and Modern Portfolio Theory to construct and visualize the efficient frontier of 10,000 randomly weighted portfolios consisting of AAPL, MSFT, and GOOGL.

## 📌 Objective
To identify the Sharpe-optimal portfolio allocation that maximizes return per unit of risk.

---

## 📊 Methodology

- Collected daily price data (2020–2024) using `yfinance`
- Calculated daily returns and annualized mean + covariance
- Simulated 10,000 random portfolios and calculated:
  - Expected return
  - Volatility (standard deviation)
  - Sharpe ratio (assuming risk-free rate = 0)
- Used `scipy.optimize` to compute the Sharpe-optimal portfolio
- Plotted the efficient frontier with the optimal point marked

---

## 🧠 Key Results

| Ticker | Optimal Weight |
|--------|----------------|
| AAPL   | 33%            |
| MSFT   | 42%            |
| GOOGL  | 25%            |

- **Expected Return**: ~18.2%  
- **Volatility**: ~15.5%  
- **Sharpe Ratio**: ~1.17

---

## 📈 Visualization

> The efficient frontier below shows all simulated portfolios, color-coded by Sharpe ratio. The red ⭐ marks the optimal portfolio:

*(Include the `plt.savefig()` version of your plot here if possible)*

---

## 🛠️ Tools Used

- Python: `pandas`, `numpy`, `yfinance`, `matplotlib`, `scipy.optimize`
- Platform: Google Colab
- Technique: Modern Portfolio Theory

---

## 📁 File Structure

- `portfolio_optimization_efficient_frontier.ipynb`: Full notebook
- `README.md`: This summary
- (Optional) `efficient_frontier_plot.png`: Visualization export

---

*This project is part of my quant research portfolio.*

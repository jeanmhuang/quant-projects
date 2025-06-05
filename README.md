# Fama-French 3-Factor Model Analysis: Apple Inc. (AAPL)

This project applies the Fama-French 3-Factor model to analyze Apple's daily excess returns from 2020 to 2024.

## 📈 Objective

To quantify how much of AAPL's returns can be explained by:
- Market risk (MKT-RF)
- Size premium (SMB)
- Value premium (HML)

## 🧪 Methodology

- Fetched AAPL daily returns using `yfinance`
- Retrieved Fama-French factor data from Kenneth French's data library
- Aligned dates and calculated AAPL's excess return over the risk-free rate
- Regressed excess return on the 3 factors using `statsmodels`

## 📊 Regression Results

| Coefficient | Estimate | p-value | Interpretation |
|-------------|----------|---------|----------------|
| **Alpha (const)** | 0.0006 | 0.095 | Slight positive alpha, not significant |
| **Market Beta** | 1.1873 | < 0.001 | Strong positive exposure to market returns |
| **Size Beta** | –0.3890 | < 0.001 | Large-cap characteristics |
| **Value Beta** | –0.3793 | < 0.001 | Strong tilt toward growth stocks |

- **R-squared**: 0.726  
- **Sample Size**: 1005 daily observations (2020–2024)

## 🛠️ Tools Used

- Python: `pandas`, `yfinance`, `statsmodels`, `requests`, `zipfile`
- Data: Yahoo Finance, Kenneth French Data Library

---

*This project is part of my quant portfolio.*

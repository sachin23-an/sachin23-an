# Sachin Kumar

Quantitative Research | Risk Analytics | Algorithmic Trading

IIT Madras, B.S. Data Science & Applications

[LinkedIn](https://linkedin.com/in/sachin-kumar-6b5609257) | [GitHub](https://github.com/sachin23-an)

---

## Research

**The Complexity Trap: A Comparative Analysis of Classical and Machine Learning Trading Strategies on the NIFTY 50 Index**

Working Paper | June 2026

Compared six strategies (buy-and-hold to LSTM) on NIFTY 50 over 5 years. Evaluated after realistic Indian transaction costs, not just gross returns. Result: a 10-line moving average beats a deep learning model after costs. Introduced the **Complexity Penalty** metric (Gross Sharpe minus Net Sharpe) to quantify this effect.

**Key finding:** XGBoost gross Sharpe 0.78 becomes net Sharpe 0.19 after costs. SMA crossover gross Sharpe 0.52 becomes net Sharpe 0.48. Model sophistication and real-world profitability are inversely related after transaction costs.

[Repository](https://github.com/sachin23-an/the-complexity-trap) | [Colab Notebook](https://colab.research.google.com) | [PDF](link-to-be-added)

---

## Projects

**1. the-complexity-trap**

Python | pandas | NumPy | scikit-learn | XGBoost | TensorFlow/Keras

Master Colab notebook implementing all six strategies from the research paper with cost-aware evaluation and leakage audit framework.

[Repository](https://github.com/sachin23-an/the-complexity-trap) | Status: Research

**2. backtesting-engine**

Python | pandas | NumPy | SciPy | yfinance

Vectorised SMA + Bollinger backtest with Sharpe, CAGR, MaxDD, Monte Carlo simulation. 1,000-path resampling preserving autocorrelation structure.

[Repository](https://github.com/sachin23-an/quant-journey/tree/main/backtesting-engine) | Status: Complete

**3. nifty-timeseries**

Python | statsmodels | arch | matplotlib

ADF/KPSS stationarity, ACF/PACF, ARIMA, GARCH(1,1) volatility. 5-day ahead forecast with 95% CI. Validated with Ljung-Box test.

[Repository](https://github.com/sachin23-an/quant-journey/tree/main/nifty-timeseries) | Status: Complete

**4. options-pricer**

Python | NumPy | SciPy | matplotlib

Black-Scholes from scratch, analytical Greeks, Newton-Raphson IV solver, 3D IV surface. No QuantLib dependency.

[Repository](https://github.com/sachin23-an/quant-journey/tree/main/options-pricer) | Status: Complete

**5. pairs-trading**

Python | statsmodels | SciPy | pandas

Engle-Granger cointegration, OLS hedge ratio, z-score signals, walk-forward backtest. FDR correction on 25 stock pairs.

[Repository](https://github.com/sachin23-an/quant-journey/tree/main/pairs-trading) | Status: Complete

**6. var-dashboard**

Python | NumPy | SciPy | matplotlib | seaborn

4-method VaR + CVaR: Historical, Parametric, Monte Carlo, Cornish-Fisher. 2x2 comparison matrix. Cornish-Fisher included for leptokurtic NSE distributions.

[Repository](https://github.com/sachin23-an/quant-journey/tree/main/var-dashboard) | Status: Complete

**7. ml-for-quant**

Python | scikit-learn | XGBoost | pandas

Next-day direction prediction with 17 engineered features. TimeSeriesSplit validation, leakage audit, feature selection on training data only.

[Repository](https://github.com/sachin23-an/quant-journey/tree/main/ml-for-quant) | Status: Complete

---

## Skills

**Languages:** Python (advanced), SQL, Bash/Linux

**Data & ML:** pandas, NumPy, SciPy, statsmodels, scikit-learn, XGBoost, TensorFlow/Keras, feature engineering, time-series validation, hyperparameter tuning

**Quant Finance:** Black-Scholes, Greeks, implied volatility, VaR (4 methods), CVaR, Monte Carlo simulation, ARIMA, GARCH, cointegration, walk-forward analysis, backtesting

**Tools:** Git, GitHub, Jupyter, Google Colab, yfinance

**Credentials:** Bloomberg BMC, NISM Series VIII (Equity Derivatives), NISM Series XV (Research Analyst), SUNY Practical Time Series Analysis

---

## Education

**B.S. in Data Science and Applications | IIT Madras**

2023 - 2027 (expected)

---

## Awards

- First Place - Mathematics, IIT Madras Paradox'23
- Founder & Secretary - Boundless, IITM BS Travel & Community Society (4,000+ members)

---

## Contact

LinkedIn: [linkedin.com/in/sachin-kumar-6b5609257](https://linkedin.com/in/sachin-kumar-6b5609257)

GitHub: [github.com/sachin23-an](https://github.com/sachin23-an)

Location: Dhanbad, Jharkhand | Open to remote roles and relocation

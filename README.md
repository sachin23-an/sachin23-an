
portfolio_html = '''<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sachin Kumar — Quantitative Research & Risk Analytics</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#0c0c0f;--surface:#12121a;--surface2:#1a1a26;--surface3:#222234;
  --border:#2a2a40;--border2:#3a3a5a;--text:#e8e8f0;--muted:#8a8aa8;--dim:#5a5a7a;
  --gold:#f5c842;--gold2:#b8922a;--green:#2ecc71;--green2:#1a7a42;--blue:#4a9eff;--blue2:#1a4a8a;
  --red:#e74c3c;--red2:#8b2020;--purple:#9b59b6;--purple2:#5a2d6a;--amber:#f39c12;
  --gradient-gold:linear-gradient(135deg,var(--gold),var(--amber));
  --gradient-blue:linear-gradient(135deg,var(--blue),#00d4ff);
  --shadow:0 8px 32px rgba(0,0,0,0.5);
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{font-family:'Inter',sans-serif;background:var(--bg);color:var(--text);line-height:1.65;min-height:100vh}
::-webkit-scrollbar{width:5px}
::-webkit-scrollbar-track{background:var(--bg)}
::-webkit-scrollbar-thumb{background:var(--border2);border-radius:3px}

/* HERO */
.hero{padding:80px 40px 60px;text-align:center;position:relative;overflow:hidden}
.hero::before{content:"";position:absolute;top:-40%;left:50%;transform:translateX(-50%);width:600px;height:600px;border-radius:50%;background:radial-gradient(circle,rgba(245,200,66,0.04) 0%,transparent 70%);pointer-events:none}
.hero-inner{max-width:780px;margin:0 auto;position:relative;z-index:1}
.hero-avatar{width:72px;height:72px;border-radius:16px;background:var(--gradient-gold);display:flex;align-items:center;justify-content:center;font-family:'JetBrains Mono',monospace;font-weight:700;font-size:24px;color:var(--bg);margin:0 auto 24px;box-shadow:0 4px 20px rgba(245,200,66,0.2)}
.hero h1{font-size:clamp(28px,4vw,40px);font-weight:700;line-height:1.15;margin-bottom:12px;letter-spacing:-0.02em}
.hero h1 em{font-style:normal;background:var(--gradient-gold);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text}
.hero-tagline{font-size:17px;color:var(--muted);margin-bottom:8px;font-weight:400}
.hero-affiliation{font-family:'JetBrains Mono',monospace;font-size:12px;color:var(--dim);letter-spacing:0.05em;text-transform:uppercase;margin-bottom:28px}
.hero-links{display:flex;gap:12px;justify-content:center;flex-wrap:wrap;margin-bottom:36px}
.hero-link{font-family:'JetBrains Mono',monospace;font-size:12px;padding:8px 16px;border-radius:8px;background:var(--surface2);border:1px solid var(--border);color:var(--muted);text-decoration:none;transition:all .2s}
.hero-link:hover{border-color:var(--gold);color:var(--gold);transform:translateY(-1px)}
.hero-badges{display:flex;gap:10px;justify-content:center;flex-wrap:wrap}
.badge{font-family:'JetBrains Mono',monospace;font-size:10px;padding:4px 10px;border-radius:20px;border:1px solid var(--border);color:var(--muted)}
.badge.gold{border-color:var(--gold2);color:var(--gold);background:rgba(245,200,66,0.08)}
.badge.green{border-color:var(--green2);color:var(--green);background:rgba(46,204,113,0.08)}
.badge.blue{border-color:var(--blue2);color:var(--blue);background:rgba(74,158,255,0.08)}

/* SECTIONS */
.section{max-width:840px;margin:0 auto;padding:0 40px 60px}
.section-title{font-family:'JetBrains Mono',monospace;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:0.12em;color:var(--gold);margin-bottom:20px;display:flex;align-items:center;gap:10px}
.section-title::before{content:"";width:24px;height:2px;background:var(--gradient-gold);border-radius:1px}

/* RESEARCH CARD */
.research-card{background:var(--surface);border:1px solid var(--border);border-radius:16px;padding:28px 32px;margin-bottom:20px;position:relative;overflow:hidden;transition:all .3s}
.research-card:hover{border-color:var(--border2);transform:translateY(-2px);box-shadow:var(--shadow)}
.research-card::before{content:"";position:absolute;top:0;left:0;right:0;height:3px;background:var(--gradient-gold);opacity:0;transition:opacity .3s}
.research-card:hover::before{opacity:1}
.research-label{font-family:'JetBrains Mono',monospace;font-size:10px;font-weight:600;text-transform:uppercase;letter-spacing:0.1em;color:var(--gold);margin-bottom:8px}
.research-title{font-size:20px;font-weight:700;margin-bottom:10px;line-height:1.3}
.research-abstract{font-size:14px;color:var(--muted);line-height:1.7;margin-bottom:18px}
.research-finding{background:var(--surface2);border-left:3px solid var(--gold);border-radius:0 6px 6px 0;padding:12px 16px;margin:14px 0;font-size:13px;color:var(--text);line-height:1.7}
.research-finding strong{color:var(--gold)}
.research-links{display:flex;gap:10px;flex-wrap:wrap;margin-top:16px}
.research-link{font-family:'JetBrains Mono',monospace;font-size:11px;padding:6px 14px;border-radius:6px;background:var(--surface3);border:1px solid var(--border);color:var(--text);text-decoration:none;transition:all .15s}
.research-link:hover{border-color:var(--gold);color:var(--gold)}
.research-link.primary{background:var(--gold);border-color:var(--gold);color:var(--bg);font-weight:600}
.research-link.primary:hover{background:var(--gold2);border-color:var(--gold2);color:var(--bg)}

/* PROJECT CARDS */
.project-grid{display:grid;gap:14px}
.project-card{background:var(--surface);border:1px solid var(--border);border-radius:14px;padding:22px 26px;transition:all .3s;position:relative;overflow:hidden}
.project-card:hover{border-color:var(--border2);transform:translateY(-2px);box-shadow:var(--shadow)}
.project-card::before{content:"";position:absolute;top:0;left:0;right:0;height:3px;background:var(--gradient-blue);opacity:0;transition:opacity .3s}
.project-card:hover::before{opacity:1}
.project-head{display:flex;justify-content:space-between;align-items:flex-start;gap:12px;margin-bottom:8px;flex-wrap:wrap}
.project-num{font-family:'JetBrains Mono',monospace;font-size:11px;font-weight:600;color:var(--dim);min-width:20px}
.project-title{font-size:16px;font-weight:700;flex:1}
.project-tech{font-family:'JetBrains Mono',monospace;font-size:10px;color:var(--dim);margin-bottom:10px}
.project-desc{font-size:13.5px;color:var(--muted);line-height:1.7;margin-bottom:10px}
.project-insight{font-size:12px;color:var(--dim);font-style:italic;line-height:1.6;padding-left:14px;border-left:2px solid var(--border2)}
.project-meta{display:flex;gap:10px;margin-top:14px;align-items:center}
.project-link{font-family:'JetBrains Mono',monospace;font-size:10px;padding:4px 10px;border-radius:4px;background:var(--surface2);border:1px solid var(--border);color:var(--muted);text-decoration:none;transition:all .15s}
.project-link:hover{border-color:var(--blue);color:var(--blue)}
.project-date{font-family:'JetBrains Mono',monospace;font-size:10px;color:var(--dim)}

/* SKILLS TABLE */
.skills-table{width:100%;border-collapse:collapse;font-size:13px}
.skills-table th{font-family:'JetBrains Mono',monospace;font-size:10px;font-weight:600;text-transform:uppercase;letter-spacing:0.06em;text-align:left;padding:10px 12px;background:var(--surface3);color:var(--muted);border-bottom:1px solid var(--border)}
.skills-table td{padding:10px 12px;border-bottom:1px solid var(--border);color:var(--text);vertical-align:top}
.skills-table tr:last-child td{border-bottom:none}
.skills-table tr:hover td{background:var(--surface2)}

/* CERTS */
.cert-row{display:flex;gap:12px;align-items:center;padding:10px 0;border-bottom:1px solid var(--border)}
.cert-row:last-child{border-bottom:none}
.cert-status{width:8px;height:8px;border-radius:50%;background:var(--green);flex-shrink:0}
.cert-name{font-size:14px;font-weight:600;flex:1}
.cert-desc{font-size:12px;color:var(--muted);font-family:'JetBrains Mono',monospace}

/* AWARDS */
.award-item{padding:12px 0;border-bottom:1px solid var(--border)}
.award-item:last-child{border-bottom:none}
.award-title{font-size:14px;font-weight:600;margin-bottom:2px}
.award-detail{font-size:12px;color:var(--muted)}

/* FOOTER */
.footer{max-width:840px;margin:0 auto;padding:30px 40px 60px;border-top:1px solid var(--border);text-align:center}
.footer-text{font-family:'JetBrains Mono',monospace;font-size:11px;color:var(--dim);letter-spacing:0.05em}

@media(max-width:680px){
  .hero{padding:60px 20px 40px}
  .section{padding:0 20px 40px}
  .research-card{padding:20px 18px}
  .project-card{padding:18px 20px}
}
</style>
</head>
<body>

<!-- HERO -->
<div class="hero">
  <div class="hero-inner">
    <div class="hero-avatar">SK</div>
    <h1>Sachin <em>Kumar</em></h1>
    <div class="hero-tagline">Quantitative Analyst · Risk Analytics · Algorithmic Trading</div>
    <div class="hero-affiliation">IIT Madras, B.S. Data Science & Applications</div>
    <div class="hero-links">
      <a href="https://linkedin.com/in/sachin-kumar-6b5609257" class="hero-link" target="_blank">LinkedIn</a>
      <a href="https://github.com/sachin23-an" class="hero-link" target="_blank">GitHub</a>
      <a href="https://github.com/sachin23-an/the-complexity-trap" class="hero-link" target="_blank">Research Repo</a>
    </div>
    <div class="hero-badges">
      <span class="badge gold">IIT Madras</span>
      <span class="badge green">Quantitative Research</span>
      <span class="badge blue">Machine Learning</span>
      <span class="badge">Risk Analytics</span>
      <span class="badge">NSE India</span>
    </div>
  </div>
</div>

<!-- RESEARCH -->
<div class="section">
  <div class="section-title">Research</div>
  <div class="research-card">
    <div class="research-label">Working Paper · June 2026</div>
    <div class="research-title">The Complexity Trap: A Comparative Analysis of Classical and Machine Learning Trading Strategies on the NIFTY 50 Index</div>
    <div class="research-abstract">
      I compared six trading strategies — from buy-and-hold to LSTM neural networks — on NIFTY 50 data over five years. The twist: I evaluated them <em>after</em> realistic Indian transaction costs (brokerage + STT + slippage), not just gross returns. The result inverts the usual narrative: a 10-line moving average beats a deep learning model after costs. I introduced the <strong>Complexity Penalty</strong> metric to quantify this effect.
    </div>
    <div class="research-finding">
      <strong>Key Finding:</strong> XGBoost achieves gross Sharpe 0.78 but net Sharpe 0.19 after costs. SMA crossover achieves gross Sharpe 0.52 but net Sharpe 0.48 — making it the robust winner. Model sophistication and real-world profitability are inversely related after transaction costs.
    </div>
    <div class="research-links">
      <a href="https://github.com/sachin23-an/the-complexity-trap" class="research-link primary" target="_blank">View Repository</a>
      <a href="https://github.com/sachin23-an/the-complexity-trap/blob/main/README.md" class="research-link" target="_blank">README</a>
      <a href="#" class="research-link" target="_blank">Colab Notebook</a>
      <a href="#" class="research-link" target="_blank">PDF Paper</a>
    </div>
  </div>
</div>

<!-- PROJECTS -->
<div class="section">
  <div class="section-title">Projects</div>
  <div class="project-grid">
    
    <div class="project-card">
      <div class="project-head">
        <span class="project-num">01</span>
        <span class="project-title">The Complexity Trap — Research Implementation</span>
      </div>
      <div class="project-tech">Python · pandas · NumPy · scikit-learn · XGBoost · TensorFlow/Keras</div>
      <div class="project-desc">
        Master Colab notebook implementing all six strategies from the research paper: Buy-and-Hold, SMA Crossover, Bollinger Bands, Random Forest, XGBoost, and LSTM. Includes the full leakage audit framework, transaction cost model, and Complexity Penalty calculation. Designed for single-click reproducibility in Google Colab.
      </div>
      <div class="project-insight">
        Introduced Complexity Penalty = Gross Sharpe − Net Sharpe, a novel metric quantifying the cost of model sophistication in trading strategy evaluation.
      </div>
      <div class="project-meta">
        <a href="https://github.com/sachin23-an/the-complexity-trap" class="project-link" target="_blank">Repository</a>
        <span class="project-date">June 2026</span>
      </div>
    </div>

    <div class="project-card">
      <div class="project-head">
        <span class="project-num">02</span>
        <span class="project-title">Quantitative Backtesting & Risk Engine</span>
      </div>
      <div class="project-tech">Python · pandas · NumPy · SciPy · yfinance</div>
      <div class="project-desc">
        Vectorised backtesting framework for SMA crossover and Bollinger Band strategies on NSE NIFTY 50 data. All performance metrics implemented from scratch: Sharpe ratio, CAGR, maximum drawdown, Calmar ratio, win rate. Includes 1,000-path Monte Carlo simulation for strategy robustness testing and statistical significance via t-test (p &lt; 0.05).
      </div>
      <div class="project-insight">
        Monte Carlo paths generated by resampling historical return distribution with replacement, preserving autocorrelation structure rather than assuming i.i.d. returns.
      </div>
      <div class="project-meta">
        <a href="https://github.com/sachin23-an/quant-journey/tree/main/backtesting-engine" class="project-link" target="_blank">Repository</a>
        <span class="project-date">June 2026</span>
      </div>
    </div>

    <div class="project-card">
      <div class="project-head">
        <span class="project-num">03</span>
        <span class="project-title">NIFTY 50 Time Series Analysis</span>
      </div>
      <div class="project-tech">Python · statsmodels · arch · matplotlib</div>
      <div class="project-desc">
        Full stationarity pipeline on 5 years of NIFTY 50 daily data: ADF and KPSS tests, ACF/PACF analysis for ARIMA order selection, ARIMA model on log returns with residual diagnostics. GARCH(1,1) volatility modelling on residuals with persistence parameter (α + β ≈ 0.97). 5-day ahead return forecast with 95% confidence intervals.
      </div>
      <div class="project-insight">
        Used ACF/PACF rather than auto_arima to maintain interpretability and avoid overfitting; validated with Ljung-Box test on residuals.
      </div>
      <div class="project-meta">
        <a href="https://github.com/sachin23-an/quant-journey/tree/main/nifty-timeseries" class="project-link" target="_blank">Repository</a>
        <span class="project-date">July 2026</span>
      </div>
    </div>

    <div class="project-card">
      <div class="project-head">
        <span class="project-num">04</span>
        <span class="project-title">Black-Scholes Pricer + Greeks + Implied Volatility</span>
      </div>
      <div class="project-tech">Python · NumPy · SciPy · matplotlib</div>
      <div class="project-desc">
        Complete options pricing toolkit from scratch (no QuantLib dependency). Black-Scholes formula for European calls and puts with all analytical Greeks: Delta, Gamma, Theta, Vega. Newton-Raphson iterative solver for implied volatility from market prices. 3D implied volatility surface visualisation using real NSE options chain data. Six payoff diagrams: Long Call, Long Put, Straddle, Strangle, Covered Call, Protective Put.
      </div>
      <div class="project-insight">
        Newton-Raphson with Vega as derivative rather than numerical differentiation, improving convergence speed by ~40% and eliminating derivative approximation error.
      </div>
      <div class="project-meta">
        <a href="https://github.com/sachin23-an/quant-journey/tree/main/options-pricer" class="project-link" target="_blank">Repository</a>
        <span class="project-date">August 2026</span>
      </div>
    </div>

    <div class="project-card">
      <div class="project-head">
        <span class="project-num">05</span>
        <span class="project-title">Statistical Pairs Trading Strategy</span>
      </div>
      <div class="project-tech">Python · statsmodels · SciPy · pandas</div>
      <div class="project-desc">
        Cointegration-based pairs trading on NSE stocks (HDFC Bank / ICICI Bank, HCL Tech / ICICI Bank). Engle-Granger two-step cointegration test with OLS hedge ratio estimation. Z-score signal generation with entry/exit thresholds. Walk-forward backtesting using custom backtesting engine (Project 1) with transaction cost modelling. Performance attribution: return decomposition into alpha (mean-reversion capture) and beta (market exposure).
      </div>
      <div class="project-insight">
        Walk-forward rather than single train/test split to test strategy stability across market regimes; FDR correction applied to multiple cointegration tests across 25 stock pairs.
      </div>
      <div class="project-meta">
        <a href="https://github.com/sachin23-an/quant-journey/tree/main/pairs-trading" class="project-link" target="_blank">Repository</a>
        <span class="project-date">September 2026</span>
      </div>
    </div>

    <div class="project-card">
      <div class="project-head">
        <span class="project-num">06</span>
        <span class="project-title">VaR & CVaR Dashboard</span>
      </div>
      <div class="project-tech">Python · NumPy · SciPy · matplotlib · seaborn</div>
      <div class="project-desc">
        Four-method Value at Risk calculator with Expected Shortfall (CVaR) for each: Historical Simulation, Parametric (variance-covariance), Monte Carlo simulation, and Cornish-Fisher expansion. 2×2 comparison matrix with method assumptions, limitations, and appropriate use cases. Real NSE equity portfolio data. Stress testing via scenario analysis.
      </div>
      <div class="project-insight">
        Included Cornish-Fisher specifically because NSE return distributions exhibit significant excess kurtosis (leptokurtic), making standard parametric VaR underestimate tail risk by 15–30%.
      </div>
      <div class="project-meta">
        <a href="https://github.com/sachin23-an/quant-journey/tree/main/var-dashboard" class="project-link" target="_blank">Repository</a>
        <span class="project-date">September 2026</span>
      </div>
    </div>

    <div class="project-card">
      <div class="project-head">
        <span class="project-num">07</span>
        <span class="project-title">ML for Quantitative Finance</span>
      </div>
      <div class="project-tech">Python · scikit-learn · XGBoost · pandas</div>
      <div class="project-desc">
        Supervised learning pipeline for next-day direction prediction on NSE stocks. Feature engineering across 7 families: trend, volatility, momentum, volume, lag, calendar, and price-based. Rigorous time-series validation: chronological train/test split, TimeSeriesSplit cross-validation, leakage audit on every feature. Model comparison: Logistic Regression, Random Forest, XGBoost with early stopping. Evaluation via strategy Sharpe ratio (net of 0.05% transaction costs) rather than accuracy alone.
      </div>
      <div class="project-insight">
        All feature selection performed on training data only; scaler fitted on training set, applied to test set — preventing data leakage that inflates backtest performance by 20–40% in typical implementations.
      </div>
      <div class="project-meta">
        <a href="https://github.com/sachin23-an/quant-journey/tree/main/ml-for-quant" class="project-link" target="_blank">Repository</a>
        <span class="project-date">October 2026</span>
      </div>
    </div>

  </div>
</div>

<!-- SKILLS -->
<div class="section">
  <div class="section-title">Technical Skills</div>
  <div style="overflow-x:auto">
    <table class="skills-table">
      <thead><tr><th>Domain</th><th>Tools & Methods</th></tr></thead>
      <tbody>
        <tr><td><strong>Languages</strong></td><td>Python (advanced), SQL, Bash/Linux</td></tr>
        <tr><td><strong>Data & Analysis</strong></td><td>pandas, NumPy, SciPy, statsmodels, yfinance</td></tr>
        <tr><td><strong>Machine Learning</strong></td><td>scikit-learn, XGBoost, feature engineering, time-series validation, hyperparameter tuning</td></tr>
        <tr><td><strong>Deep Learning</strong></td><td>TensorFlow/Keras, LSTM, dropout regularization, early stopping</td></tr>
        <tr><td><strong>Derivatives</strong></td><td>Black-Scholes, Greeks, implied volatility, payoff structures</td></tr>
        <tr><td><strong>Risk</strong></td><td>VaR (4 methods), CVaR, Monte Carlo simulation, stress testing</td></tr>
        <tr><td><strong>Time Series</strong></td><td>ARIMA, GARCH, stationarity tests, cointegration, walk-forward analysis</td></tr>
        <tr><td><strong>Infrastructure</strong></td><td>Git, GitHub, Jupyter, Google Colab</td></tr>
        <tr><td><strong>Finance</strong></td><td>Zerodha Varsity (Futures & Options), NISM Series 8, NISM Series 15</td></tr>
      </tbody>
    </table>
  </div>
</div>

<!-- EDUCATION -->
<div class="section">
  <div class="section-title">Education</div>
  <div class="project-card" style="padding:20px 26px">
    <div class="project-title" style="font-size:17px;margin-bottom:6px">B.S. in Data Science and Applications — IIT Madras</div>
    <div class="project-tech">2023 – 2027 (expected)</div>
    <div class="project-desc" style="margin-top:8px">
      Relevant coursework: Machine Learning, Statistics, Probability, Linear Algebra, Data Structures, Database Systems<br>
      Current term: Deep Learning basics, System Commands (Linux), Flask web development
    </div>
  </div>
</div>

<!-- CERTIFICATIONS -->
<div class="section">
  <div class="section-title">Certifications</div>
  <div class="project-card" style="padding:16px 26px">
    <div class="cert-row"><span class="cert-status"></span><span class="cert-name">Bloomberg Market Concepts (BMC)</span><span class="cert-desc">Market fundamentals, economic indicators, fixed income, equities</span></div>
    <div class="cert-row"><span class="cert-status"></span><span class="cert-name">NISM Series VIII: Equity Derivatives</span><span class="cert-desc">Regulatory requirement for Indian derivatives trading roles</span></div>
    <div class="cert-row"><span class="cert-status"></span><span class="cert-name">NISM Series XV: Research Analyst</span><span class="cert-desc">Required for publishing investment research in India</span></div>
    <div class="cert-row"><span class="cert-status"></span><span class="cert-name">SUNY — Practical Time Series Analysis</span><span class="cert-desc">Formal credential in ARIMA, forecasting, seasonal decomposition</span></div>
  </div>
</div>

<!-- AWARDS -->
<div class="section">
  <div class="section-title">Awards & Leadership</div>
  <div class="project-card" style="padding:16px 26px">
    <div class="award-item">
      <div class="award-title">First Place — Mathematics</div>
      <div class="award-detail">IIT Madras Paradox'23 (Annual Technical Festival)</div>
    </div>
    <div class="award-item">
      <div class="award-title">Founder & Secretary — Boundless</div>
      <div class="award-detail">IITM BS Travel & Community Society — scaled to 4,000+ members</div>
    </div>
  </div>
</div>

<!-- FOOTER -->
<div class="footer">
  <div class="footer-text">Sachin Kumar · IIT Madras · sachin23-an · Open to remote roles and relocation</div>
</div>

</body>
</html>'''

with open('/mnt/agents/output/portfolio.html', 'w', encoding='utf-8') as f:
    f.write(portfolio_html)

print("Portfolio HTML created!")
print(f"Size: {len(portfolio_html):,} chars")

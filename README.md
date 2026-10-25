Defense Contractors: Risk & Return Analysis (2015–2024)

This is a quantitative study of how five of the largest U.S. defense contractors have behaved as investments over ten years. It looks at their volatility, tail risk, drawdowns, market sensitivity and reaction to events, and compares each one with the S&P 500.

Why Defense?

Defense primes are usually seen as defensive holdings. They have long government contracts, multi-year backlogs and demand that doesn't depend much on the economy. This project tests that idea with data. It asks whether these stocks really move less with the market, recover faster from selloffs and react less to shocks than the broader market does.

The Companies
Ticker	Company	Core Business
NOC	Northrop Grumman	Aerospace, space systems, strategic deterrence
LMT	Lockheed Martin	Combat aircraft (F-35), missiles, space
RTX	RTX Corp. (Raytheon)	Missile defense, aircraft engines, avionics
BA	Boeing	Commercial aircraft and defense/space
GD	General Dynamics	Submarines, combat vehicles, Gulfstream jets
SPY	S&P 500 ETF	Market benchmark

Boeing is included on purpose. Its large commercial-aviation business makes it a useful comparison to the pure defense names, especially through COVID-19 and the 737 MAX crisis.

What the Analysis Covers
Return distributions: mean, volatility, skew and kurtosis, with Jarque-Bera tests for normality and a ranking of fat tails.
Drawdowns: the largest peak-to-trough loss, how long the decline took and when (or whether) each stock recovered.
Value at Risk: historical and parametric VaR, plus CVaR (expected shortfall), at 95% confidence.
Market sensitivity: beta, alpha and correlation to SPY, plus a 60-day rolling correlation.
Volatility dynamics: 20- and 60-day rolling volatility and autocorrelation of returns and squared returns, to test for volatility clustering.
Fear gauge: how each stock's rolling volatility tracks the VIX.
Event effects: the size of price moves on earnings days and on high-volume days compared with normal days.
Performance: cumulative growth of $1 against the benchmark.
Tools

Python · pandas · NumPy · SciPy · statsmodels · matplotlib · seaborn · yfinance

How to Run
bash
pip install yfinance pandas numpy scipy statsmodels matplotlib seaborn
jupyter notebook defense_contractors_analysis.ipynb
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ari-price/Defense-Financial-Analytics/blob/main/defense_contractors_analysis.ipynb)

Price, volume, earnings and VIX data come from Yahoo Finance through yfinance. To analyze a different basket or period, change tickers, start and end in the configuration cell.

Notebook Structure
Configuration: tickers, benchmark, date range and risk settings
Data retrieval: prices, volumes, VIX and earnings dates
Analysis functions: statistics, risk metrics and correlations
Visualization functions: charts for each metric
Results: tables and figures

Ari Price · B.S. International Business & Finance, University of San Diego, Knauss School of Business

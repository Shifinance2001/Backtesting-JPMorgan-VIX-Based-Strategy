# JPMorgan VIX Buy Signal — Backtest & Analysis

## 📰 Strategy Overview
JPMorgan's research team identified a rules-based market timing indicator with a claimed **100% accuracy rate outside of recessions** over three decades.

- **The Signal:** Buy the S&P 500 when the **Cboe Volatility Index (VIX)** closes more than **50% above its 1-month (30-day) rolling moving average**

- **Signal Cooldown:** Signals within 30 days of a prior signal are ignored, preventing repeated triggering during sustained volatility.

- **Exit Rule:** Hold for **6 months** after each signal, then measure the S&P 500 return.

- **Result from JPMorgan's analysis:**
1. Triggered **21 times** since 1990
2. Average S&P 500 return of **~9%** in the 6 months following each signal
3. All positive outcomes occurred **outside of recession periods**

## 📊 Backtest Results (1990–2022)
 
| Metric | Value |
|---|---|
| Signal triggers (1990–2022) | **21** |
| Average 6-month S&P 500 return (excl. last 2) | **~+7.9%** |
| Worst signal (2008 GFC recession) | **~-32.7%** |
| Strategy accuracy outside recessions | **~100%** |

> The two recession-era signals (notably the 2008 financial crisis) are the exceptions where the signal failed — confirming JPMorgan's caveat that the indicator works *outside* recessions.

## ⚠️ Limitations & Caveats
 
- **Recession caveat:** JPMorgan explicitly noted the signal fails during recessions. The 2008 GFC signal produced a ~-33% drawdown over the following 6 months.
- **Lookahead bias:** This is a backtest — forward performance is not guaranteed.
- **Small sample size:** 21 signals over 32 years is a limited dataset.
- **Data source:** Uses Yahoo Finance data via `yfinance`, which may differ slightly from Bloomberg terminal data used in the original research.
- **No transaction costs:** This backtest does not account for slippage, commissions, or taxes.

 ## 📚 References
 
- Bloomberg article: https://www.bloomberg.com/news/articles/2022-02-08/jpmorgan-strategists-see-sure-fire-sign-it-s-time-to-buy-stocks

# 📰 Original Bloomberg Article

- (bloomberg_article_text_1.png)
![Bloomberg Article Continued](bloomberg_article_text_2.png)
![JPMorgan VIX Chart](bloomberg_vix_chart.png)

## 🔧 Disclaimer
The trading strategy described in this repository is based on publicly reported research by JPMorgan strategists as covered in a Bloomberg article (February 2022). This project is an independent educational replication and is **not affiliated with, endorsed by, or sponsored by JPMorgan Chase & Co. or Bloomberg**.


 

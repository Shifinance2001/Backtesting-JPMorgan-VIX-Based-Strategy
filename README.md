# JPMorgan VIX Buy Signal — Backtest & Analysis

## 📰 Strategy Overview
JPMorgan's research team identified a rules-based market timing indicator with a claimed **100% accuracy rate outside of recessions** over three decades.

**The Signal:**
> Buy the S&P 500 when the **Cboe Volatility Index (VIX)** closes more than **50% above its 1-month (30-day) rolling moving average**

**Signal Cooldown:** Signals within 30 days of a prior signal are ignored, preventing repeated triggering during sustained volatility.

**Exit Rule:** Hold for **6 months** after each signal, then measure the S&P 500 return.

 
**Result from JPMorgan's analysis:**
- Triggered **21 times** since 1990
- Average S&P 500 return of **~9%** in the 6 months following each signal
- All positive outcomes occurred **outside of recession periods**

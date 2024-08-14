# 🌀 Mean Reversion Strategy: DJIA Backtesting Adventure

Welcome to the *Mean Reversion Strategy* project, where we delve into the wild world of trading by betting on the underdogs of the Dow Jones Industrial Average (DJIA). This project backtests a mean reversion strategy, pitting it against the big bad Dow Jones ETF (DIA) to see who comes out on top.

## 🧐 What's All This About?

In the realm of finance, mean reversion is the idea that asset prices and returns tend to return to their historical averages over time. So, when stocks take a nosedive, we swoop in, buy them up, and (hopefully) profit when they bounce back. This project explores just how effective this strategy is when applied to the DJIA constituents over a 10-year period.

## 💡 Project Highlights

- **Data Acquisition**: We grab the latest list of DJIA constituents from Wikipedia (because why not?) and fetch 10 years of daily adjusted close prices using the `yfinance` library. All data is safely stashed in CSV files, and we handle any hiccups along the way with grace and poise (and a little error handling).
  
- **Strategy Implementation**:
  - **Daily Returns Calculation**: We start by calculating daily returns for each stock.
  - **Identifying the Biggest Losers**: Each day, we pick the 10 stocks that took the biggest hits (poor things) and get ready to place our bets.
  - **Trade Simulation**: We simulate buying these sad stocks at the close of the day and selling them at the close of the next day, starting with a cool $100,000.
  - **Performance Metrics**: Annualized return, volatility, Sharpe ratio (fancy finance talk for risk-adjusted returns), and maximum drawdown are calculated to see if our strategy's got what it takes.
  - **Comparison with the Dow Jones Index**: We put our strategy head-to-head with the DIA ETF to see who reigns supreme.
  - **Visualizing Portfolio Growth**: Watch the magic happen as we graph the growth of our $100,000 portfolio over time.

## 🛠️ System Requirements

To join this financial adventure, you’ll need:

- Python 3.x
- `pandas` (for data wrangling)
- `yfinance` (for fetching all that sweet, sweet stock data)
- `numpy` (because math)
- `plotly` (for making everything look pretty)

## 🚀 How to Run This Project

1. **Clone the Repository**: 
    ```bash
    git clone https://github.com/yourusername/mean-reversion-djia.git
    cd mean-reversion-djia
    ```

2. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Main Script**:
    ```bash
    python mean_reversion_strategy.py
    ```

4. **Watch the Magic Unfold**: Sit back, relax, and let the script do its thing. By the end, you'll have a detailed comparison of how our mean reversion strategy fared against the DIA ETF.

## 📊 Results & Findings

After all is said and done, we analyze the performance metrics to determine if betting on the biggest losers was a winning strategy. Spoiler alert: sometimes the underdogs really do have their day. We also provide some snazzy graphs to visualize the portfolio growth over time.

## 🤔 Concluding Observations

This project is a deep dive into the potential profitability of a mean reversion strategy applied to the DJIA. The results, visualizations, and metrics provide valuable insights into whether this approach can hold its own against the broader market. Plus, you get the added thrill of seeing if your strategy can outsmart the Dow!

## 📜 License

There isn’t one! This project is free to use, modify, and share—just don’t blame us if you lose your shirt trading stocks! 😅

---

Happy trading! May your returns be ever in your favor.

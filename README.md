# Pairs Trading and Cointegration Strategy

## Project Overview

**Project Title:** Pairs Trading and Cointegration Strategy   


This project implements a market-neutral pairs trading strategy using statistical techniques such as correlation and cointegration to identify and trade highly correlated stock pairs. The approach is designed to exploit mean-reverting relationships between stocks, aiming for consistent returns regardless of overall market direction.

## Description

Pairs trading is a form of statistical arbitrage that involves identifying two stocks with a historically strong correlation. When the price relationship between these stocks diverges beyond a certain threshold, the strategy takes offsetting long and short positions, betting on the spread to revert to its historical mean. The project covers:

- **Pair Identification:** Using correlation coefficients, p-values, and stationarity tests (ADF) to select suitable stock pairs.
- **Signal Generation:** Employing moving averages and z-scores to generate entry and exit signals.
- **Risk Management:** Implementing stop-loss and take-profit mechanisms, and optimizing position sizing based on regression coefficients.
- **Backtesting:** Evaluating the strategy on out-of-sample data to assess performance using metrics like CAGR, Sharpe ratio, and maximum drawdown.

## Implications

- **Market Neutrality:** The strategy is designed to profit in both rising and falling markets, reducing exposure to overall market risk.
- **Statistical Rigor:** By relying on cointegration and stationarity tests, the approach ensures that only robust, mean-reverting pairs are traded.
- **Risk Management:** Incorporates dynamic position sizing and stop-loss mechanisms to minimize downside risk and optimize returns.
- **Automation:** The entire workflow, from data acquisition to signal generation and performance evaluation, is automated using Python and relevant libraries.

## Application

### 1. **Quantitative Trading**
- Enables traders and quantitative analysts to systematically identify and exploit arbitrage opportunities in equity markets.
- Can be extended to other asset classes (ETFs, commodities, currencies) with minor modifications.

### 2. **Portfolio Diversification**
- Adds a market-neutral component to investment portfolios, potentially reducing overall volatility and drawdowns.

### 3. **Educational Use**
- Serves as a comprehensive case study for students and professionals learning about statistical arbitrage, time series analysis, and algorithmic trading.

### 4. **Research and Development**
- Provides a foundation for further research into advanced strategies, such as multi-asset pairs trading, machine learning-based pair selection, and high-frequency trading adaptations.

## Key Features

- **Data Acquisition:** Automated fetching of historical stock data using Yahoo Finance API.
- **Statistical Analysis:** Correlation, cointegration, and stationarity testing for robust pair selection.
- **Signal Generation:** Moving average and z-score based entry/exit logic.
- **Risk Controls:** Stop-loss, take-profit, and dynamic position sizing.
- **Performance Metrics:** Calculation of CAGR, Sharpe ratio, maximum drawdown, and trading frequency.
- **Visualization:** Plots for correlation matrices, trading signals, and portfolio performance.

## Getting Started

1. **Clone the Repository:**  
   Download or clone the project files from GitHub.

2. **Install Dependencies:**  
   Ensure Python and required libraries (pandas, numpy, matplotlib, seaborn, yfinance, statsmodels, scikit-learn) are installed.

3. **Run the Code:**  
   Execute the provided Jupyter notebooks or Python scripts to fetch data, select pairs, generate signals, and backtest the strategy.

4. **Analyze Results:**  
   Review the generated plots and performance metrics to evaluate strategy effectiveness.

## Example Use Cases

- **Backtesting on US Tech Stocks:**  
  Apply the strategy to a basket of technology stocks (e.g., AAPL, MSFT, GOOGL) to identify profitable pairs and trading opportunities.

- **Risk Management Demonstration:**  
  Showcase how stop-loss and position sizing mechanisms protect against large losses during adverse market movements.

- **Performance Reporting:**  
  Generate reports summarizing cumulative returns, Sharpe ratio, and drawdown for different pairs and time periods.

## References

- "Pairs Trading: Quantitative Methods and Analysis" by Ganapathy Vidyamurthy
- "Statistical Arbitrage: Algorithmic Trading Insights and Techniques" by Andrew Pole
- [Investopedia: Pairs Trading](https://www.investopedia.com/terms/p/pairs_trade.asp)


**For questions, contributions, or collaboration, please open an issue or submit a pull request on GitHub.**

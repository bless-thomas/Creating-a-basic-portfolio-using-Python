# Stock Portfolio Optimization Using Risk Scoring and Modern Portfolio Theory (MPT)
## Project Overview
This project implements a stock portfolio optimization tool that categorizes stocks into risk portfolios based on a combination of fundamental and technical analysis. The tool uses Modern Portfolio Theory (MPT) to generate optimal portfolios that maximize returns for a given level of risk. By leveraging financial metrics, technical indicators, and sector-specific benchmarks, the project aims to match stocks to an investor's risk appetite and provide a final portfolio with the best risk-adjusted returns.

## Key Features
### Risk Scoring Based on Fundamental and Technical Factors:
The tool calculates a risk score for each stock based on factors such as:

### Fundamental Indicators: Debt-to-Equity (DE) Ratio, Price-to-Earnings (PE) Ratio, Return on Equity (ROE), Return on Capital Employed (ROCE), Market Capitalization, etc.
### Technical Indicators: Relative Strength Index (RSI), Moving Average Convergence Divergence (MACD), and volatility metrics (standard deviation, mean return).
### Sector-Specific Risk Conditions:
Different sectors (e.g., Energy, Financials, Technology) have unique risk thresholds. The project accounts for this by assigning different scoring bands for financial ratios and stock behavior, ensuring that risk scores are accurate and relevant to the stock's sector.

### Portfolio Classification:
Stocks are classified into Low, Medium, and High-risk portfolios based on their calculated risk score. This allows users to create diversified portfolios tailored to their risk tolerance.

### Efficient Frontier Calculation Using MPT:
The tool uses Modern Portfolio Theory to optimize the user’s selected portfolio. It calculates the efficient frontier, which represents portfolios that offer the maximum possible return for a given level of risk.

### Risk Appetite Customization:
Based on user inputs regarding risk tolerance (e.g., low, medium, or high risk), the tool automatically selects a suitable portfolio and optimizes it to match the user's investment goals.

### Technologies Used
Python: For implementing the overall solution and handling data processing.
pypfopt Library: To calculate portfolio weights, risk, and return using Modern Portfolio Theory (MPT).
NumPy & Pandas: For data manipulation and calculations.
Yahoo Finance API: For pulling historical stock prices and sector data.
scikit-learn: For normalizing and scaling the risk scores.
How It Works
Input:
The user provides a list of stocks, and the program fetches relevant financial data for each stock. The user also specifies their risk appetite via a survey or predefined options.

### Risk Scoring:
The tool calculates a risk score for each stock by analyzing both fundamental (financial ratios) and technical (RSI, MACD) indicators. Sector-specific thresholds are applied to ensure more accurate risk classification.

### Portfolio Classification:
Based on the calculated risk scores, stocks are divided into three categories:

Low-Risk
Medium-Risk
High-Risk

### Optimization with MPT:
The tool then optimizes the user's selected risk portfolio using Modern Portfolio Theory, generating a portfolio that lies on the efficient frontier, providing the best risk-adjusted return for the user's chosen risk level.

### Future Enhancements
Implement machine learning models for better risk prediction and classification.
Introduce real-time stock data integration for dynamic portfolio adjustments.
Expand to include global stocks and multi-asset portfolios for diversification.

# EURUSDProphet

A comprehensive mathematical and statistical exploration of EUR/USD daily returns using descriptive statistics, correlation analysis, and probabilistic inference.

## Overview

This project applies fundamental statistical and mathematical concepts to analyze the behavior and characteristics of EUR/USD exchange rate daily returns over a 5-year historical period. Rather than building predictive models, the objective is to understand the statistical properties, distributions, and relationships in financial time-series data through rigorous mathematical analysis.

## Project Objectives

1.  **Descriptive Statistics**: Analyze the distribution of daily returns (mean, variance, skewness, kurtosis, fat tails).
2.  **Bivariate Analysis**: Investigate correlations between EUR/USD and S&P 500 returns.
3.  **Central Limit Theorem**: Empirically demonstrate how sample means converge to normality.
4.  **Conditional Probability**: Test for market independence and efficiency.
5.  **Data Visualization**: Create professional visualizations of historical prices and statistical distributions.

## Project Structure

```
├── data/                    # Historical market data directory
├── models/                  # Mathematical models and analysis
├── config/                  # Configuration files
│   ├── config.py            # Project configuration constants
│   └── system_prompt.md     # Analysis guidelines (not tracked)
├── sample.ipynb             # Main Jupyter notebook with all analysis
├── README.md                # Project documentation
└── requirements.txt         # Python dependencies
```

## Installation

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)
- Virtual environment (recommended)

### Setup

1.  Clone or navigate to the project directory:
    ```bash
    cd JupyterProject1
    ```

2.  Create and activate a virtual environment:
    ```bash
    python -m venv .venv
    .venv\Scripts\activate  # On Windows
    source .venv/bin/activate  # On macOS/Linux
    ```

3.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

Open the Jupyter notebook to view the complete analysis:

```bash
jupyter notebook sample.ipynb
```

The notebook is organized into the following sections:
1.  Data Overview and Sources
2.  Historical Price Data Visualization
3.  Descriptive Statistics of Daily Returns
4.  Bivariate Analysis: Covariance and Correlation
5.  Central Limit Theorem Simulation
6.  Probability and Conditional Probability Analysis
7.  Conclusions and Limitations

## Data Source

All historical daily data was obtained from **Yahoo Finance** using the `yfinance` Python library:
- **EUR/USD** (ticker: EURUSD=X): Exchange rate between Euro and US Dollar
- **S&P 500** (ticker: ^GSPC): US stock market index of 500 large companies
- **Period**: 5 years of historical daily closing prices
- **Frequency**: Daily market data

## Dependencies

| Package | Purpose |
|---------|---------|
| yfinance | Download historical market data from Yahoo Finance |
| pandas | Data manipulation and analysis |
| numpy | Numerical computing |
| matplotlib | Data visualization |
| seaborn | Statistical data visualization |
| scipy | Statistical functions (norm.pdf for distributions) |
| sympy | Symbolic mathematics |
| jupyter/notebook | Interactive notebook environment |

See `requirements.txt` for full dependency specifications.

## Key Findings

- **Non-Normal Returns**: EUR/USD daily returns exhibit excess kurtosis (fat tails), indicating extreme events are more frequent than a normal distribution would predict.
- **Weak Correlation**: The correlation between EUR/USD and S&P 500 daily returns is very weak, demonstrating their relative independence.
- **Market Efficiency**: Conditional probability analysis shows that past returns have negligible predictive value for future returns, supporting the Efficient Market Hypothesis.
- **CLT Validation**: Even though individual daily returns are not perfectly normal, the distribution of sample means closely follows a normal distribution.

## Limitations

- This analysis is based on **historical data** and past performance does not guarantee future results.
- The study focuses on **daily returns** only; longer-term or intraday patterns are not analyzed.
- **External factors** such as macroeconomic news, geopolitical events, and central bank policies are not explicitly modeled.
- No **predictive models** are developed; the analysis is purely descriptive and inferential.

## Future Research Directions

- Implement **ARIMA** or **GARCH** models to capture volatility clustering.
- Apply **Machine Learning** algorithms (Prophet, LSTM networks) for forecasting.
- Incorporate **macroeconomic indicators** and external features.
- Extend analysis to **multiple timeframes** (hourly, weekly, monthly).
- Conduct **regime-switching analysis** to identify market states.

## Academic Integrity

This project was developed as an academic exercise in applying mathematical and statistical concepts to real-world financial data. All data sources are publicly available and properly credited. No proprietary data or models were used.

## Author & Credits

**Project**: EURUSDProphet  
**Focus**: Mathematical and Statistical Analysis  
**Data Source**: Yahoo Finance (via yfinance library)  
**Created**: 2025-2026

## License

This project is for educational and research purposes.



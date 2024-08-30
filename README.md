

---

# Quantitative Trading Strategy for Indian Equities

This repository contains a Python implementation of data-oriented Quantitative Trading strategies focused on Indian equities. The strategy leverages a 6-year dataset to identify and trade stock pairs using statistical methods like Cointegration and Distance-Based Approaches.

## Project Overview

The primary goal of this project is to develop robust trading tactics that can identify profitable opportunities in the Indian equity markets. By employing statistical analysis and machine learning techniques, the strategy seeks to capitalize on market inefficiencies, especially through pair trading methods.

### Key Features:

- **Cointegration-Based Pair Trading**: Pinpoints stock pairs whose linear combination produces a stationary time series, ensuring profitable reversion to the mean.
- **Distance-Based Pair Trading**: Identifies pairs based on price distance metrics and historical correlation, offering an alternative to the Cointegration method.
- **Hedge Ratio Calculation**: Uses linear regression to determine the hedge ratio for optimal capital allocation between paired stocks.
- **Signal Generation**: Employs moving averages on the normalized spread to generate buy, sell, and square-off signals for executing trades.

## Strategy Breakdown

### 1. Cointegration Approach
- **Objective**: Identify pairs of stocks that exhibit a stable, long-term relationship.
- **Process**: Cointegration testing is performed to ensure that the spread between the two stocks is mean-reverting.
- **Hedge Ratio**: Calculated through linear regression to minimize portfolio variance.
- **Signal Generation**: When the normalized spread diverges from its moving average, buy/sell signals are generated.

### 2. Distance-Based Approach
- **Objective**: Identify pairs of stocks with historically similar price movements.
- **Process**: Analyzes the distance between stock prices and historical correlation to determine potential pairs.
- **Signal Generation**: Trades are initiated when the price distance deviates from its historical norm.

## Installation

To get started, clone this repository and install the required Python packages:

```bash
git clone https://github.com/your-username/quant-trading-strategy.git
cd quant-trading-strategy
pip install -r requirements.txt
```

## Usage

### Data Preparation
- Ensure you have access to a 6-year dataset of Indian equity prices. You can obtain this from sources like Yahoo Finance or NSE.
- Place your data files in the `/data` directory.

### Running the Strategy
Run the following command to execute the trading strategy:

```bash
python main.py
```

The script will output trade signals, potential profit, and a performance summary based on historical data.

## Results

The strategy outputs the following metrics for analysis:
- Total returns and annualized returns
- Sharpe ratio
- Maximum drawdown
- Performance of individual stock pairs

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please open an issue or submit a pull request.

## Contact

For any inquiries, please contact [bhawariyajaat@gmail.com](mailto:bhawariyajaat@gmail.com).

---

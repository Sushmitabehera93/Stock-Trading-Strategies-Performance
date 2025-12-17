# Stock-Trading-Strategies-Performance

## Table of Contents
- [Project Overview](#project-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Methodology](#methodology)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
This project aims to evaluate whether technical indicator–based stock trading strategies can achieve higher performance than top-performing mutual funds offered by major Canadian financial institutions like TD.

## Installation
1. Clone the repository:
   ```
   git clone https://github.com/yourusername/Stock-Trading-Strategies-Performance.git
   ```
2. Navigate to the project directory and install dependencies:
   ```
   Use a tool like pip or poetry to install dependencies:
   pip install uv
   ```
   ```
   uv --version
   uv init
   uv add package name
   ```

## Usage
- To run the main analysis script:
  ```
  python main.py
  ```
- For interactive exploration, open the Jupyter notebook:
  ```
  StockPredictiction_Final.ipynb
  ```

## Dataset
- The project uses historical stock price data and mutual fund performance data from major Canadian financial institutions.
- Data includes daily prices, trading volumes, and technical indicators for selected stocks, as well as performance metrics for mutual funds.
- Data sources and preprocessing steps are documented in the code and notebooks.

## Project Structure
- `main.py` – Main script for running trading strategy evaluations
- `StockPredictiction_Final.ipynb` – Jupyter notebook for analysis and visualization
- `pyproject.toml` – Project metadata and dependencies
- `README.md` – Project documentation

## Methodology

### 3.1. Data Sources
The data was collected using Python from Yahoo Finance (Y-Finance) and includes historical daily stock data for major technology companies such as AAPL, AMZN, GOOGL, META, MSFT, NVDA, NFLX, TSLA, AVGO, and PLTR. The dataset spans multiple years (2015–2025) and contains standard OHLCV fields: Open, High, Low, Close, and Volume. Additionally, a benchmark mutual fund (TD908) was included to compare the performance of technical trading strategies against a traditional investment option.

### 3.2. Analytical Approach
The project focused on testing systematic trading strategies grouped into four main types:
- **Trend-Following Strategies:** (e.g., Moving Average Crossover, Breakout, Price Channel)
- **Momentum Strategies:** (e.g., Rate of Change (ROC), 52-Week Breakout, RSI Momentum)
- **Mean Reversion Strategies:** (e.g., Bollinger Bands, RSI Reversal, Moving Average Envelope)
- **Hybrid Strategies:** (e.g., Moving Average + RSI, Breakout + Bollinger, Momentum + Reversion Filter)

Each strategy was backtested using Python to generate buy and sell signals. Performance was evaluated using key metrics including CAGR, Total Return, Volatility, Max Drawdown, Sharpe Ratio, Win Rate, and Profit Factor.

### 3.3. Benchmark Selection
To ensure a realistic comparison, the algorithmic strategies were measured against the TD Canadian Balanced Fund (TD908). This mutual fund is widely available to Canadian retail investors and serves as a practical benchmark for assessing whether technical trading strategies can outperform a professionally managed, diversified investment option.

### 3.4. Visualization and Evaluation
Results were summarized and visualized using Python libraries such as Matplotlib and Seaborn. Graphs illustrated annual returns, performance metrics by ticker, and comparisons between the strategies and the mutual fund benchmark. These visualizations highlighted which strategies performed most consistently and how they behaved under different market conditions.

## Results

- Technical indicator–based trading strategies were tested on major technology stocks (2015–2025) and compared to the TD Canadian Balanced Fund (TD908).
- Some strategies (e.g., Bollinger Bands, RSI Reversion) performed well during strong trends or high volatility but suffered large drawdowns in downturns.
- More stable strategies (e.g., Moving Average Envelope, ROC) produced smaller but steadier gains.
- No single technical strategy consistently outperformed the mutual fund benchmark over the long term.
- Mutual funds provided more reliable and balanced results for long-term investing.
- Technical trading strategies are best used for short-term opportunities or as part of a diversified investment approach, not as full replacements for mutual funds.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for improvements or new features.

## License
This project is licensed under the MIT License.



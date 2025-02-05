# AI-Trading-Agents

This project implements AI-driven trading strategies to analyze stock market behavior using historical data from Yahoo Finance. The code focuses on high-volatility stocks such as TSLA and AMZN, leveraging adaptive moving average strategies and heuristic adjustments to optimize trading performance.

The main components include:

Single Simulation: Runs a trading strategy using AI agents with different moving average windows.
Multiple Simulations (Hypothesis Testing): Executes 50 independent simulations to evaluate the robustness of the strategy.
Features
Dynamic Moving Averages: AI agents adjust their short-term and long-term moving average windows based on market performance.
Stock Data Acquisition: Fetches historical stock prices using Yahoo Finance API.
Performance Evaluation: Tracks cumulative returns and dynamically adjusts agent strategies.
Monte Carlo Simulations: Runs multiple simulations to test the robustness of the strategy.


Installation
To run this project, install the required dependencies:
pip install pandas numpy yfinance matplotlib


Usage
Run the notebook to fetch stock data and execute AI-driven trading strategies.
Modify the ticker variable to test different stocks.
Adjust moving average parameters for different market conditions.

Results
Cumulative returns for AI agents are plotted and compared.
Final moving average windows for each agent are displayed.
Statistical analysis of multiple simulations helps assess strategy robustness.

Example Output:

Final Cumulative Returns - AMZN
Original Agent A: 1.42
Original Agent B: 1.35
Adaptive Agent A: 1.68
Adaptive Agent B: 1.52
Final windows for Agent A: {'short_window': 50, 'long_window': 220}
Final windows for Agent B: {'short_window': 45, 'long_window': 180}

Notes
This strategy is optimized for high-volatility stocks.
Adjusting segment_length changes the re-evaluation frequency.
The heuristic algorithm adapts the strategy dynamically to market trends.

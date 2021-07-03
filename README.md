# Module_5_Challenge
The application entails building a tool to help credit union members evaluate their financial health. Specifically, the credit union board wants the members to be able to do two things. First, they should be able to assess their monthly budgets. Second, they should be able to forecast a reasonably effective retirement plan based on their current holdings of cryptocurrencies, stocks, and bonds using Monte Carlo simulations.

---
## Technologies
- [Anaconda](https://www.anaconda.com/products/individual) - Pandas is included in Anaconda distribution and Conda package manager to manage Python environments.
- [Jupyter Lab](https://jupyter.org/) - web-based user interface designed for data analysis. It lets you write, run, and review the results in Python programs (all in a single integrated development environment (IDE).
- [Alpaca API](https://alpaca.markets) Unlimited access to real-time US stock market data using API keys
- [JSON](https://www.json.org/json-en.html) - This library puts the response (that is, the data) from an API into a human-readable format.
- [Requests](https://docs.python-requests.org/en/master/) - The Python Requests library helps you access data via APIs.
- [OS](https://docs.python.org/3/library/os.html) - The OS module comes under Python's standard utility models and provides functions for interacting with the computer's operating system. The OS module does not require a separate download.

---
## Installation Guide

If your development environment is missing either package, you can directly install it.
To install the Requests library, check that your development environment is active, and then run the following command:

```
conda install -c anaconda requests

```

To install the JSON library, check that your development environment is active, and then run the following command:

```
conda install -c jmcmurray json

```
With the python-dotenv library, you can read key-value pairs from an environment file (.env) and add them as environment variables.
To install this library, run the following command in your terminal:

```
pip install python-dotenv

```
Alpaca is an API for stock trading. With the Alpaca SDK, you can interact with the Alpaca API.
To install this SDK, run the following command in your terminal:

```
pip install alpaca-trade-api

```

---

## Usage

Monte Carlo Simulation Example

```
# Configure the Monte Carlo simulation to forecast 30 years cumulative returns
# The weights should be split 40% to AGG and 60% to SPY.
# Run 500 samples.

MC_thirtyyear = MCSimulation(
    portfolio_data = forecast_portfolio,
    weights = [.60, .40],
    num_simulation = 500,
    num_trading_days = 252 * 30 
)
# Review the simulation input data

MC_thirtyyear.portfolio_data.head()

```

## Contributors

Created by Bina Jariwala

---

## License

None

---

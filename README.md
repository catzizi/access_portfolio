# access_portfolio
To execute the main script,  run:
python -m portfolio.analysis
 use pandas for reading in data, calculating various statistics and plotting a comparison graph.
A portfolio is a collection of stocks (or other investment options) and corresponding allocations of money to each of them.
In order to evaluate and compare different portfolios, we first need to compute certain metrics,
based on available historical data.

The primary goal of this project is to do portfolio analysis
compute the daily portfolio value over given date range, and then the following statistics for the overall portfolio:

Cumulative return
Average daily return
Standard deviation of daily returns
Sharpe ratio of the overall portfolio, given daily risk free rate (usually 0), and yearly sampling frequency (usually 252, the no. of trading days in a year)
Ending value of the portfolio
Where the returned outputs are:

cr: Cumulative return
adr: Average daily return
sddr: Standard deviation of daily return
ev: End value of portfolio
The input parameters are:

sd: A datetime object that represents the start date
ed: A datetime object that represents the end date
syms: A list of symbols that make up the portfolio (note that your code should support any symbol in the data directory)
allocs: A list of allocations to the stocks, must sum to 1.0
sv: Start value of the portfolio
rfr: The risk free rate for the entire period
sf: Sampling frequency per year
gen_plot: If True, create a plot named plot.png

# Efficient Frontier — Modern Portfolio Theory

A quantitative finance project exploring Markowitz's Modern Portfolio 
Theory using Monte Carlo simulation, built in Python.

## Background

Given a set of assets with different returns and risks, what is the 
optimal way to split your money between them? Markowitz's answer- published in 1952 and awarded the Nobel Prize — is to consider not just individual asset properties but how assets move together.

The key insight is diversification: combining assets that are 
uncorrelated or negatively correlated reduces portfolio volatility 
without sacrificing return. 

## The Model

For a portfolio with weights $\mathbf{w}$, expected return and 
volatility are:

$$\mu_p = \mathbf{w}^T \boldsymbol{\mu}$$

$$\sigma_p = \sqrt{\mathbf{w}^T \Sigma \mathbf{w}}$$

where $\Sigma$ is the covariance matrix capturing how assets move 
together.

## What the Notebook Contains

- Four simulated stocks with different risk/return profiles
- Correlation heatmap showing diversification relationships
- Monte Carlo simulation of 10,000 random portfolios
- Efficient frontier visualisation coloured by Sharpe ratio
- Optimal (maximum Sharpe) portfolio identification
- Minimum variance portfolio identification
- Summary table of optimal portfolio weights

## Key Results

### Correlation Structure
![Correlation Heatmap](images/correlation_heatmap.png)

Stocks 2 and 3 are slightly negatively correlated- they provide 
the best diversification benefit when combined.

### The Efficient Frontier
![Efficient Frontier](images/efficient_frontier.png)

Each dot is one randomly generated portfolio. The glowing yellow 
edge is the efficient frontier- the set of portfolios that deliver 
maximum return for a given level of risk. The red star marks the 
optimal Sharpe portfolio and the blue cross marks the minimum 
variance portfolio.

Notice that all four individual stocks sit inside the cloud- 
diversification always dominates holding any single asset alone.

## Main Ideas Explored

- Modern Portfolio Theory and mean-variance optimisation
- Diversification and the covariance matrix
- Monte Carlo simulation of portfolio space
- The efficient frontier as the boundary of optimal portfolios
- Sharpe ratio as a measure of risk-adjusted performance
- Maximum Sharpe vs minimum variance portfolios

## Tools

- Python
- NumPy
- Matplotlib
- Pandas

## Author

Yarin Negyal — first year Mathematics student at the University of 
Warwick, interested in quantitative finance and stochastic processes.

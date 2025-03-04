# Heston Model vs. Black-Scholes Forecasting Using Real Apple Market Data

This project compares the Heston Model and the Black-Scholes Model for forecasting options prices using real market data from Apple Inc. (AAPL). The project involves data preprocessing, model implementation, and analysis of the results. **Note: The predictions from the models have not yet been compared with real market data.**

## Table of Contents
- [Introduction](#introduction)
- [Data Preprocessing](#data-preprocessing)
- [Models](#models)
- [Results](#results)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [License](#license)
- [Acknowledgments](#acknowledgments)
- [Contact](#contact)

## Introduction
The goal of this project is to compare the effectiveness of the Heston Model and the Black-Scholes Model in forecasting options prices using real market data from Apple Inc. The project involves:
- Downloading and preprocessing options and stock data
- Implementing both pricing models
- Analyzing and visualizing results

**Important Note:** The predictions from these models have not yet been validated against real market data.

## Data Preprocessing

### Data Collection
- Downloaded historical options and stock data for AAPL using `yfinance`
- Collected multiple expiration dates and strike prices
- Retrieved implied volatility surfaces

### Data Cleaning
- Handled missing values and outliers
- Calculated time-to-expiration (T) in years
- Filtered in-the-money (ITM) and out-of-the-money (OTM) options
- Normalized and scaled relevant features

### Key Features
- Strike prices ranging from $50 to $450
- Expiration dates from March 2025 to June 2027
- Implied volatility surfaces
- Daily historical stock prices

## Models

### Black-Scholes Model
- Implements the classic options pricing formula
- Assumes constant volatility
- Calculates theoretical prices using:
  - Current stock price
  - Strike price
  - Risk-free rate
  - Time to expiration
  - Historical volatility

### Heston Model
- Stochastic volatility model
- Accounts for volatility smile/skew
- Parameters include:
  - Long-term volatility
  - Mean reversion rate
  - Volatility of volatility
  - Correlation between asset and volatility

## Results
**Current Status:** Model predictions have been generated but not yet compared with real market data for validation.

Planned analysis will include:
- Volatility surface comparisons
- Pricing error metrics (RMSE, MAE)
- Residual analysis
- Model convergence tests

## Acknowledgments
Yahoo Finance API for market data access
Original authors of both financial models
Contributors to Python scientific computing stack

## Contact
For questions or collaborations:
Email: brewsmith.a@northeastern.edu

Note: This is an ongoing research project. Validation against real market data and model calibration improvements are planned for future work.



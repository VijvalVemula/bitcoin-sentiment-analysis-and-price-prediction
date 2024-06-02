# Project Overview

This project aims to predict the future price of Bitcoin using historical price data and Wikipedia edit data related to the Bitcoin page. By merging and analyzing this data, we'll train a random forest model to predict whether Bitcoin prices will increase or decrease the following day. Later, we'll enhance the model by switching to an XGBoost model and refining our predictors to improve accuracy.

We'll also develop a backtesting system and use a robust error metric to evaluate the algorithm's performance. This methodology can be applied to other cryptocurrencies as well.

**Project Steps**

1. Load the data.
2. Clean and merge the data.
3. Create an initial machine learning model and estimate its accuracy.
4. Transition to a more powerful model and improve the predictors.

## Code

You can find the project code on [GitHub](https://github.com/VijvalVemula/bitcoin-sentiment-analysis-and-price-prediction).

File overview:

- `price-prediction.ipynb` - Contains the code for predicting Bitcoin prices.
- `sentiment-analysis.ipynb` - Creates the Wikipedia edit dataset.

# Local Setup

## Installation

To follow this project, please install the following locally:

- JupyterLab
- Python 3.8+
- Required Python packages:
  - pandas
  - yfinance
  - scikit-learn
  - xgboost
  - mwclient
  - transformers

## Data

Generating the Wikipedia edit data can be time-consuming, so it's recommended to use the pre-generated version available in the repository, named `wiki_edits.csv`. You can also download it from [this link](https://drive.google.com/uc?export=download&id=1XwJZ07bl2u-62yRMqV_emJGEXCI1u8dl).

We'll use the `yfinance` package to download the Bitcoin price data as part of the project.

## Running

1. Run the code in `sentiment-analysis.ipynb` to generate a new Wikipedia edits dataset. The committed dataset is outdated, and this step ensures it includes the latest edits.
2. Execute the code in `price-prediction.ipynb`. By default, it loads data from an existing `btc.csv` file. Removing this code will ensure it downloads the latest data from Yahoo Finance.

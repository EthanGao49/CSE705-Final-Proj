# Stock Price Forecasting using LSTM

This project uses LSTM and Mixture of Experts (MoE) models to perform forecasting on Apple (AAPL) stock prices. The workflow is implemented in a single Jupyter Notebook and covers data loading, model training, evaluation, and visualization.

## Required Packages

Make sure you have the following Python packages installed:

- numpy
- pandas
- tensorflow
- scikit-learn
- yfinance
- matplotlib

## How to Run

1. Open `proj.ipynb` in Jupyter Notebook/VS Code/Google Colab.
2. Run all cells in order (Run All).

The notebook will automatically download data using Yahoo Finance's API, train models, display results and plots.
Tips: Google Colab is recommended as all required package has already been installed.

## Contents

- Data loading and preprocessing
- Baseline LSTM model
- Mixture of Experts (MoE) model
- Multi-scale Temporal MoE model
- Plot: Training and validation loss curves
- Plot: Short-term and long-term prediction 

To reproduce the results, simply run all cells. No extra configuration is needed.

---

## Experiment Summary

| Model                        |    RMSE    |    MAE    |
|------------------------------|:----------:|:---------:|
| Baseline LSTM                | 10.1948    | 8.3756    |
| Mixture of Experts (MoE)     |  6.0760    | 4.6295    |
| Multi-scale Temporal MoE     |  4.9886    | 3.5304    |

- Multi-scale Temporal MoE achieved the best overall performance, with the lowest MAE and RMSE.
- The MoE model improves overall trend prediction compared to the baseline LSTM.
- The Multi-scale Temporal MoE introduces short-horizon experts, making the model more sensitive to price fluctuation in short-term


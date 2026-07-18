# Stock Price Prediction with PyTorch (LSTM & GRU)

A deep learning project that predicts Apple (AAPL) stock closing prices using **Long Short-Term Memory (LSTM)** and **Gated Recurrent Unit (GRU)** neural networks implemented with **PyTorch**.

The project demonstrates the complete workflow of a time-series forecasting task, including data collection, preprocessing, model training, evaluation, and comparison.

---

# Features

- Download historical stock data using **yfinance**
- Data preprocessing and normalization
- Sliding window sequence generation
- LSTM implementation with PyTorch
- GRU implementation with PyTorch
- Performance evaluation using:
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - Mean Absolute Error (MAE)
- Comparison of LSTM and GRU models
- Visualization of predictions

---

# Technologies

- Python
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- yfinance
- Jupyter Notebook

---

# Dataset

- **Stock:** Apple Inc. (AAPL)
- **Source:** Yahoo Finance
- **Library:** yfinance
- **Date Range:** 2015-01-01 → 2024-12-31

Only the **Closing Price** was used for prediction.

---

# Deep Learning Models

## LSTM

- Input Size: 1
- Hidden Size: 64
- Number of Layers: 2
- Dropout: 0.2
- Optimizer: Adam
- Loss Function: Mean Squared Error

---

## GRU

- Input Size: 1
- Hidden Size: 64
- Number of Layers: 2
- Dropout: 0.2
- Optimizer: Adam
- Loss Function: Mean Squared Error

---

# Evaluation Metrics

The models are evaluated using:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)

The comparison results are exported as:

```text
data/model_comparison.csv
```

---

# Project Structure

```text
stock-price-prediction-pytorch/
│
├── data/
│   └── model_comparison.csv
│
├── images/
│   └── lstm_vs_gru_prediction.png
│
├── models/
│   ├── lstm_model.pth
│   └── gru_model.pth
│
├── notebooks/
│   └── stock_price_prediction.ipynb
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

# Prediction Result

After training, both LSTM and GRU predictions are compared against the actual stock prices.

> The prediction graph is available in:

```text
images/lstm_vs_gru_prediction.png
```

---

# Installation

Clone the repository:

```bash
git clone https://github.com/metegurkaynak/stock-price-prediction-pytorch.git
```

Enter the project folder:

```bash
cd stock-price-prediction-pytorch
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
notebooks/stock_price_prediction.ipynb
```

---

# Requirements

Main libraries used:

- torch
- pandas
- numpy
- matplotlib
- scikit-learn
- yfinance

---

# Learning Outcomes

This project demonstrates:

- Time Series Forecasting
- Data Preprocessing
- Feature Scaling
- Sequence Generation
- LSTM Networks
- GRU Networks
- Deep Learning with PyTorch
- Model Evaluation
- Data Visualization

---

# Future Improvements

- Predict multiple stocks simultaneously
- Hyperparameter optimization
- Bidirectional LSTM
- Transformer-based forecasting
- Real-time prediction dashboard
- Deployment with Streamlit

---

# License

This project is released under the MIT License.

---

# Disclaimer

This project is intended for educational purposes only and should not be considered financial or investment advice.
# forecast-future-stock-values
It was to implement stock price forecasting using both  traditional statistical and machine learning methods and evaluate their performance  under a rolling window evaluation framework. This approach simulates real-world  forecasting situations where models are continuously retrained on the most recent  data before predicting the next move.

We experimented with both ARIMA (traditional statistical model) and LSTM (deep learning model) to compare performance.

Implemented models
ARIMA (p,d,q) — selected via manual grid search
LSTM (3-layer architecture) with dropout + early stopping
Both models were trained and evaluated on a stock dataset (date, close) using an 80/20 train-test split and a rolling evaluation.

Evaluation metrics
RMSE (root mean square error)
MAPE (mean absolute percent error)
Accuracy (%) = 100 - MAPE
Example results:
| Model | RMSE | MAPE (%) | Accuracy (%) |

|--------|-------|------| | ARIMA | ~6.63 | ~1.62 | ~98.4 |

| LSTM | ~8–10 | ~2–3 | ~97 |

Lower RMSE/MAPE = better performance.

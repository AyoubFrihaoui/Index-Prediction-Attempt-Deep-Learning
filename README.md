# Index Prediction Attempt Using Deep Learning

## Overview
This project is an attempt to predict stock index prices using various deep learning techniques, specifically focusing on:

- **MLP (Multilayer Perceptron)**
- **CNN1D (1D Convolutional Neural Networks)**
- **LSTM (Long Short-Term Memory Networks)**

The input features and structure used for prediction include:

- **Using 30 days in the past to predict 10 days in the future**
- **Prices**
- **Moving Averages**
- **Price Differences**


### Conclusion
After extensive testing, it has become clear that using only prices, moving averages, and price differences as features from the dataset is **insufficient for accurately predicting index prices**, regardless of the deep learning method used. The inherent complexity of financial markets makes it difficult to forecast based on these limited features alone.

Among the models tested, the **MLP** yielded the best results in terms of minimizing the Mean Squared Error (MSE) loss during forecasting. However, even the MLP's performance was inadequate for practical use.

### Key Takeaways
- **Predicting index prices using these features does not provide meaningful results to real-world cases**, highlighting the limitations of the dataset and feature selection.
- Despite the MLP's better performance compared to CNN1D and LSTM, it still falls short of delivering accurate predictions for stock index prices.

## Repository Contents
- `CSV files/` : The dataset used for training and testing.
- `* Model(s)/` : Contains the model architectures for MLP, CNN1D, and LSTM.
- `notebooks` : Jupyter notebooks showcasing the experiments and results.
- `results` : Logs and performance metrics for each model.

## Conclusion
This project serves as a learning experience in deep learning techniques applied to financial data, but the results underscore the limitations of using basic price-based features for stock index forecasting. Future work should explore more sophisticated features and models to tackle this challenging problem.


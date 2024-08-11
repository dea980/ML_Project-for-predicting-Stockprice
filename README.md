# Introduction to Artificial Intelligence 2023: Stock Market Price Prediction with AI Models

**Authors:** Daeyeop Kim, Antony Doves, and Chima Philips  
**Institution:** School of Informatics, Computing, and Engineering, Indiana University, Bloomington, IN, USA  
**Date:** 2023

## Abstract

This project explores the use of AI models to predict stock market price trends. We aim to identify which machine learning architecture provides the most accurate predictions. We evaluated several models, including LSTM, GRU, a hybrid of LSTM and GRU, Lasso, and MLP, to determine their efficacy in predicting stock trends.

## Keywords

- Stock
- Prices
- Prediction

## Problem and Data Description

Our goal is to identify correlations in historical stock data and apply AI models to predict stock price trends. We used a dataset from Yahoo! Finance containing columns such as Date, Open, High, Low, Adj Close, and Volume, focusing primarily on the Open and Close columns. The models tested include LSTM, GRU, LSTM + GRU, Lasso, and MLP.

## Data Preprocessing & Research Process

### Checking Missing Values

The dataset used for training was sourced from Yahoo! Finance, and it did not contain missing values, allowing for smooth data preprocessing.

### Research Process

We explored several regression models to find the best fit for stock price prediction. Initial trials with Lasso and MLP showed limited success, prompting a focus on sequential data models like LSTM and GRU. We then compared these models based on their ability to predict trends using both Open and Close price data.

## Algorithm and Methodology

### Models Used

1. **Lasso and MLP:** Initial attempts with these models were overfitted and not suitable for predicting sequential data.
   
2. **LSTM:** Known for capturing long-term dependencies, LSTM models include a "forget gate" for enhanced stability.

3. **GRU:** Simplified compared to LSTM, GRUs handle recurrency with two types of gates, but face challenges with short memory and gradient issues.

4. **Hybrid Model (LSTM + GRU):** Combines the strengths of LSTM and GRU, aiming to improve performance and accuracy.

## Experiments and Results

We conducted experiments to compare the Mean Squared Error (MSE) of LSTM, GRU, and the hybrid model using both Open and Close datasets:

- **Open MSE:**
  - LSTM: 490.41
  - GRU: 250.37
  - Hybrid: 643.01

- **Close MSE:**
  - LSTM: 206.38
  - GRU: 286.31
  - Hybrid: 336.57

Results indicate that GRU performed best on the Open dataset, while LSTM excelled with the closed dataset. These findings suggest variability in model performance depending on data features.

## Summary and Conclusions

The study aimed to predict stock trends using AI models. LSTM and GRU demonstrated strong capabilities for modeling sequential data, though results varied across different datasets. The GRU model showed superior performance with Open data, while LSTM excelled with closed data. Our research highlights the sensitivity of models to hyperparameters and suggests the need for further refinement to improve predictive accuracy.

## References

- [LSTM Introduction](https://www.analyticsvidhya.com/blog/2021/03/introduction-to-long-short-term-memory-lstm/)
- [GRU Explanation](https://datascience.stackexchange.com/questions/14581/when-to-use-gru-over-lstm)

## Contact

For further information, please contact Daeyeop Kim at [kdea989@gmail.com].

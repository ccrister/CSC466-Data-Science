# CSC466-Data-Science

Project Overview

The objective of this project was to develop and evaluate two models for predicting GameStop's share prices. This involved using TensorFlow and Keras to implement the models and adjust their parameters to optimize predictions.

Models
1. Recurrent Neural Network (RNN) with LSTM
Architecture: Consists of three LSTM layers followed by a dense layer.
Function: Utilizes past share price data to learn trends and make future price predictions.
Implementation: Built using TensorFlow and Keras.
2. Decision Tree Model
Method: Employs a recursive algorithm to process the dataset, making decisions at each node until a prediction is output.
Details: Implemented to compare its performance against the RNN model.
Results
Performance Variability: Testing across different stocks revealed significant variations in accuracy, influenced by external factors affecting companies.
Hyperparameter Tuning: Adjustments in the RNN's hyperparameters, like the number of epochs and LSTM units, significantly affected its performance.
Future Work
News Impact Analysis: Future iterations could explore the impact of news headlines on share prices, an aspect not covered due to time constraints.

Installation
Install the necessary packages with the following commands:

pip install --upgrade pandas pandas-datareader yfinance
Usage
Prepare your environment and data with the following imports and setups:

python
Copy code
import numpy as np
import pandas as pd
import yfinance as yf
from keras.models import Sequential
from keras.layers import LSTM, Dropout, Dense
from sklearn.tree import Decision TreeRegressor
Data for the models is sourced from Yahoo Finance using the yfinance library, which ensures the data is up-to-date and reliable for training and testing purposes.


# AI HW

Use an RNN to model bitcoin closing prices. Model 1 will use FNG fear and greed indicators to predict the closing price. Model 2 will use a window of closing prices to predict the nth closing price.

You will need to:

1. [Prepare the data for training and testing](#prepare-the-data-for-training-and-testing)
2. [Build and train custom LSTM RNNs](#build-and-train-custom-lstm-rnns)
3. [Evaluate the performance of each model](#evaluate-the-performance-of-each-model)

- - -

### Files

[Closing Prices Starter Notebook](Starter_Code/lstm_stock_predictor_closing.ipynb)

[FNG Starter Notebook](Starter_Code/lstm_stock_predictor_fng.ipynb)

- - -

## Instructions

### Prepare the data for training and testing

Use the starter code to create a Jupyter Notebook for each RNN.

For the FNG RNN, use FNG values to predict closing prices.

For the closing price RNN, use historical closing prices to predict the next closing price.

Do a 70-30 data split.

Scale the X and y values using a MinMaxScaler.

Reshape the X_train and X_test values to fit the model's requirement of samples, time steps, and features. (*example:* `X_train = X_train.reshape((X_train.shape[0], X_train.shape[1], 1))`)

### Build and train custom LSTM RNNs

In each Notebook, create the same custom LSTM RNN architecture. In Model 1, fit the data using the FNG values. In Model 2, fit the data using only closing prices.

Use the same parameters and training steps for each model, to compare the models.

### Evaluate the performance of each model

Use the testing data to evaluate each model and compare the performance.

Answer:

> Which model has a lower loss?
>
> Which model tracks the actual values better over time?
>
> Which window size works best for the model?


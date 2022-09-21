# Stock-Price-Prediction

## Stock price prediction
This is a Machine Learning algorithm to predict if the stock price will increase the next day (tomorrow). We only want to buy the stock on days when the price will go up (we're against shorting the stock).

If the algorithm says that the price will increase, we'll buy the stock
If the algorithm says that the price will go down, we won't do anything.
We want to maximize our true positives - days when the algorithm predicts that the price will go up, and it actually goes go up. Therefore, we'll be using precision as our error metric for our algorithm, which is true positives / (false positives + true positives). This will ensure that we minimize how much money we lose with false positives (days when we buy the stock, but the price actually goes down).

This means that we will have to accept a lot of false negatives - days when we predict that the price will go down, but it actually goes up. This is okay, since we'd rather minimize our potential losses than maximize our potential gains.

## Method
Download historical stock prices from Yahoo finance
Explore the data
Setup the dataset to predict future prices using historical prices
Test a machine learning model
Setup a backtesting engine
Improve the accuracy of the model
Document some potential future directions we can go in to improve the technique

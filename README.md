# Predicting the football match winner using LSTM model of Recurrent Neural Networks

This repository contains the code for a conference paper **"Predicting the football match winner using LSTM model of Recurrent Neural Networks"** that we wrote. This paper gives an introduction to the advantages of using an LSTM (Long Short-Term Memory) Cell in a Recurrent Neural Network and uses it to predict the outcome of a football match.

## Dataset 

The dataset used here has been obtained from [football-data.co.uk](http://football-data.co.uk/data.php). Datasets of the English Premier league have been taken from seasons 2010-11 to 2016-17.

## Data Preprocessing

The files [dataCleaning.ipynb](dataCleaning.ipynb) and [fdManipulate.ipynb](fdManipulate.ipynb) take the raw data from the website and add attributes regarding the win streaks and the loss streaks for every team. Also, [eplStandings.csv](datasets/eplStandings.csv) contains the final ranks of all the teams in the English Premier League from 2010-11 to 2016-17.

## Prediction

The file [LSTM.ipynb](LSTM.ipynb) [Depricated] constructs a RNN using the LSTM cell (tensorflow 1.14) and predicts the outcome of the [test dataset](allAtt_onehot_large_test.csv).

The file [LSTM_New.ipynb](LSTM_New.ipynb) constructs a RNN using the LSTM cell (tensorflow keras API) and predicts the outcome of the [test dataset](allAtt_onehot_large_test.csv).

## Result

This model proved to be better than the other models previously used to predict the winner of a football match. Detailed analysis is given in the [paper](Set_Paper.pdf) (under review).

## Libraries Required
1. tensorflow
2. pandas
3. numpy
4. datetime
5. itertools
6. scikit-learn
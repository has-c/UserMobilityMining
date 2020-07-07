# User Mobility Mining

This study was conducted from Nov 2019 to Feb 2020 at the University of Auckland under supervision by Dr Kaiqi Zhao. 

The User Mobility Mining project is about predicting the type of place (POI category) a user has visited given the spatio-temporal features of the check-in. In our study a feed-forward neural network (ANN), long short-term memory network (LSTM) and XGBOOST models were tested against one
another and then compared against the reported accuracies. The novelty of our study are the improvements in the modelling in the spatial and temporal dimensions. To improve temporal modelling we have used a time-aware LSTM. The time-aware LSTM can capture the temporal dynamics of sequential data with
time irregularities. To improve spatial modelling, we have included a geographical token feature. This feature was created by partitioning a geographical land map into grids (100 metres by 100 metres) and then assigning check-ins to these grids. Thus, each check-in was given an independent grid token, but nearby grids should have correlations. The models were tested on the publicly available gowalla dataset and four-square.

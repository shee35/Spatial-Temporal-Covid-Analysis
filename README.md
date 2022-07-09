# About the Project 
Our objective of this project is the spatial-temporal distribution of COVID 19 data and its
prediction in the nearby areas. The outbreak of COVID 19 in India claimed the lives of
thousands of people. Our main objective is to use such a strong statistical model in order
to show that COVID 19 infection is spatially dependent and is mainly spread via to the
neighboring areas.

# Proposed Methodology
Firstly, we would take a dataset of states of India, and then we would identify the hotspot
state among them. Then we will scrap the data of cities/districts of that state.
After scraping and cleaning the data we would apply the above-described strategy to
analyze and visualize data of neighboring cities. Then we will select a center among
those cities where the covid cases are the highest, then we would further use the data in
order to train our model for prediction, and test its accuracy, and optimality.

We have chosen the LSTM model because it is an extension of the Recurrent Neural
Network. And as for the covid data we know that the data is not completely independent
of itself, it depends on past data as well as the cases of areas around the hotspot, i.e. the
ones highly correlated. LSTM uses the previous data to predict the future value. Thus it
does not leave any important aspect or external factor that may drastically affect the
prediction of future cases.


# Conclusion
We have analyzed the spatial as well as the temporal spread of COVID 19 in India.  We   have taken the data from March 2020 to September 2021, and have observed the number of cases rise exponentially in different states of India especially during April-May 2020. With the infection growth and the doubling rate of COVID 19.

We found that Maharashtra is the most affected region in India by covid. Since, on plotting the Correlation Matrix amongst the different states of India, Maharashtra was found to be the hotspot of COVID cases.
In Maharashtra, district Osmanabad is most spatially temporally related to other neighbouring districts. Although pune contributes the most when it comes to the spreading of covid, due to its close proximity to Mumbai, highest daily covid cases, presence of international airports, it is also an industrial city. But for prediction, we choose Osmanabad here due to its spatial-temporal relation being highest resulting in the most accurate prediction.
LSTM with spatial-temporal data is the most accurate model among all implemented models.
If we apply our model to any district which is highly spatially temporally related to neighbouring districts, then our model is applicable to it and gives very accurate results.


| Errors   |      Spatial Temporal LSTM      |  SVM |  BiLSTM | LSTM | GRU |
|----------|:-------------|-------------------------|--------|-------|-----|
| RMSE |  0.08550 | 1.3569 | 0.1749 | 0.2979 | 0.1643 |
| MAE |    0.08537 |   0.9814 | 3.0569 | 4.8004 | 2.8725 |








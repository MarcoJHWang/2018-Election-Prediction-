# 2018-Election-Prediction-
MinneMUDAC 2018 competition

The goal is to predict number of votes cast for each party in the following 2018 elections in Minnesota
* The 8 United States House of Representatives seats 
* The 2 United States Senate seats
* The governor race 
So in total, the submission will be 33 predictions.

1. Collect data
Start by facing the most challenging and time-consuming part is data since the host of MinneMUDAC did not provide any dataset which means participant has to collect data from historical elections. Even during data collection phase, it remains lots of questions which kind of data would be useful on prediction. In final, the dataset is composed of three components in below. 

First, considering demographic factor is key for prediction; hence, most of demographic data sources from below website.
American Fact Finder: https://factfinder.census.gov/faces/nav/jsf/pages/index.xhtml

The other helpful information is the past election results, that is to say, the number of votes casted for each parties in previous elections. Here is another useful website for votes data.
Office of the Minnesota Secretary of the State: https://www.sos.state.mn.us/

One last thing is using public's opinions and tendency to aid prediction because social media is playing an important role to have an unneglectable influence. Our approach is to text mining Tweets and calculate the difference of sentiment score between two major parties, Republican and Democratic. 

2. Feature selection
Due to high dimensionality in our dataset, prediction results in highly overfitting. So, in order to reduce this phenomenon, we adopt some feature selection approaches to leave out usefl features, also PCA is adopted to reduce the dimension of predictor variables.

3. Modeling
Been running several predictive models, finally, predictions are made of average across different model's prediction. 

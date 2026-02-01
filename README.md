# WiDS_Nikhil_Kocherry
This is a compilation of the two assignments done till date. They include code regarding both ARIMA and LSTM models, and their implementation in Python.

## Week 1
This program is written to implement the ARIMA model on a data set downloaded from yfinance. 
The dataset was 'AAPL' Close prices for several months. The first part of the code was dedicated to dropping all the irrelevant data, and bringing it into Dataframe form.
We then proceed to find the best order required for ARIMA model and the dataset, by testing for the least value of the likellihood function for different values of the triplet (p,q,r).
After that, we create an ARIMA model to take the optimal order and the training dataset, and give us results to certain test data.
We then fit the model results with the actual corresponding y values for the test data, We can then see how our model did.
We analyse the residuals also using the last part of the code.

## Week 2
This program was meant to implement both ARIMA and LSTM models on the same dataset, which is the same as the one we used for the previous assignment.
This time, we take the dataset into a Forecaster object from ScaleCast, which makes testing multiple models fofr the same train and test data much more convenient.
The way we get the ARIMA model here is almost identical, and we fit this model onto our Forecaster object.
We now use the manual_forecast() function to create and LSTM model with specifications enough to make it reasonably powerful. The function automatically fits our data to this model.
We now compare the predictions given by both models on the same dataset, and analyse the errors and residual plots for the predicted data.

## Week 3 
The final piece of the puzzle involved using the TextBlob module in Python to analyze news articles related to stock prices and incorporate this information into the model training process. TextBlob provides a simple and intuitive interface for performing natural language processing tasks, making it well suited for sentiment analysis of textual data. As a first step, basic implementation of TextBlob was carried out to determine the polarity of each statement, which indicates whether the sentiment expressed in the text is positive, negative, or neutral. This polarity score helped quantify the general market sentiment conveyed by news articles.

## That was it for the WiDS Bootcamp!

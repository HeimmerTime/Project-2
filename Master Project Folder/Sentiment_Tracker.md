# Ethereum Sentiment Tracker
![Ethereum](https://thumbor.forbes.com/thumbor/fit-in/900x510/https://www.forbes.com/advisor/wp-content/uploads/2021/03/ethereum-1.jpeg)

## Project Overview

* Use Python API's to scrape Reddit comments and news headlines then convert into a usable .csv format.
* Train a model using our collected data to predict market sentiment
* Use our model on near-term data to determine market conditions

## API's and Text Acquisition
In Jupyter Lab, we utilized pre-built Python api’s to scrape text data from Ethereum-focused sources. 

- Reddit posts & comments gathered from r/Ethtrader, r/Ethereum and r/EthFinance
- We used Rakuten API to gather News Headlines across the internet with mention of Ethereum 

After the data was gathered, imported and cleaned we applied Bull market, Bear market, or neutral market conditions to each data point based on the market condition at the time of post. 

## Predictive Models
We used Vader and SKlearn as our predictive models. We chose to use Vader because it requires less training data and is efficient at decoding and quantifying emotions contained in text. 

## Reddit Model Evaluation
Vader vs. SKlearn Results

After building an LSTM model and running our data through the model we found-
- Vader was 62% accurate/correlated in testing the model for market conditions
Sklearn Accuracy/Reliability

## News Model Evaluation
Vader vs. SKlearn Results

Using our news data on the same LSTM model we found-
- Vader was 80% accurate/correlated in testing the model for market conditions
Sklearn Accuracy/Reliability

## Improvements
- Pull in more data
- Utilize other sources to reduce possible sources of bias
- Try different models to find a better fit
-Apply the model in real-time to predict current sentiment
- Plot sentiment against price to see how it lags or predicts a future price move

## Conclusion

We were able to gather enough data to train and run the model we created. We received accuracy scores over 50% and if we could gather more data and run different models we could create a more accurate sentiment prediction for Ethereum.  

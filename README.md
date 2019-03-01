# Sentiment Analysis - Text Mining
Sentiment Analysis of Twitter tweets related to 2015-16 presidential elections *to identify the various reasons for the win/loss of candidates (Trump and Clinton)* 

| Author: Divya Rajendran

## Pre-Requisites / Requirements
Python3 is needed to run this code efficiently
### Required Packages
```python
pip install jupyter pandas seaborn matplotlib preprocessor re unicodedata nltk contractions inflect textblob afinn collections wordcloud
```
Run this piece of code in terminal or cmd prompt, this will install all the required packages needed to run the jupyter notebook.

## Data
Historical tweets data is scraped from twitter using twitter API and by making use of Jefferson-Henrique/GetOldTweets-python project code.

1. *Data mined for the candidates Trump and Clinton during the period Jun 2015 - Dec 2016, one month after the results were announced for the presidential election*

2. *User opinion poll data from various websites consolidated monthly*


## Analysis
Below is a sequence of steps followed to arrive at the conclusion

1. Pre-processed tweets text to remove stop words, special characters, number, urls, hashtags, mentions and tokenized the text

2. Calculated Afinn score and sentiment polarity score using textblob based on the above tokenized words for each tweet

3. Merged user poll data with the tweets

4. Selected five variables, number of people who favorited a tweet, number of retweets, number of likes, Afinn sentiment score, and number of tweets of different polarity, to analyze the election outcome by plotting them monthly and yearly.

5. Read the plots to identify major differences between the main contendors for the presidential role.

## Conclusion & Results
When comparing all the plots for the five variables for both Trump's tweets and Clinton's tweets, we can conclude the below.

1. we find that the sentiment score remained almost the same for Clinton and there was some slow increase in the counts of three variables in consideration

2. Sentiment score for Trump was very high compared to Clinton, leading us to believe there was a lot of positive tweets made by him in 2015 when compared to 2016. Also, there was a significant increase in the counts of the three variables in consideration

3. Also, the Trump made a lot of positive tweets when compared to neutral and negative tweets in stark comparision to Clinton, who made a lot of negative tweets when compared to neutral and positive tweets

4. The word clouds we have plotted show that both the candidates spoke mostly about Trump, increasing his popularity and outreach. It might have also been one of the reasons contributing to his win.

We can say that sentiment analysis clearly tells us a lot about the electoral wins, we can try to employ similar strategies to different scenarios to understand the effect of sentiment or various other variables on the data and its target.

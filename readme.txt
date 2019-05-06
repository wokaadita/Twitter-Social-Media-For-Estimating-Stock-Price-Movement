I propose a project to analyze how Twitter can help to forecast the movement of the stock price from a particular public company.  
Rather than using news, seeing the reaction from people on Twitter will give more effective "early warning" to companies for anticipating any negative issue that might harm its businesses. It will also help the companies to identify which kind of issue that might give huge or low impact to them. Sentiment analysis could be added as well for future development.

The dataset that will be used is the historical stock price from Yahoo Finance for "Tesla" and scraping from Twitter.

# 1. Getting Dataset For Tweets

Scraping Twitter in finding dataset regarding tweet containing keyword 'Tesla'. We are using tweepy and store it in .json file. Due to very much information on it, we should pre-processing first the json file. 
Then we select several information related with the tweets itself like, number of reply, likes, retweet and the Twitter profile who tweeted it.
It's crucial to help us identified the fake account or user who is not real human(using programmed robot). Fake user tend to be just recently created. For example tweet from user accoun who was created this 2019, can be suspected as fake. In order to present the scraped tweet data nicely, we can the pre-processed result as DataFrame.
Date time also can be a problem, because I live d in Indonesia, which separated 7 hours earlier, I should adjust the time format from this dataset following my time zone.
Because twitter provide its time using GMT format as the default.


# 1. Getting Dataset For Tweets

Scraping Twitter in finding dataset regarding tweet containing keyword 'Tesla'.
We are using tweepy and store it in .json file. Due to very much information on it, we should pre-processing first the json file. Then we select several information related with the tweets itself like, number of reply, likes, retweet and the Twitter profile who tweeted it. It's crucial to help us identified the fake account or user who is not real human(using programmed robot). Fake user tend to be just recently created. For example tweet from user accoun who was created this 2019, can be suspected as fake.
In order to present the scraped tweet data nicely, we can the pre-processed result as DataFrame.
Date time also can be a problem, because I live d in Indonesia, which separated 7 hours earlier, I should adjust the time format from this dataset following my time zone. Because twitter provide its time using GMT format as the default.
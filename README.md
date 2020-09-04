# twitter-tweet-classifier-extractor
This is a repository to extract Covid 19 update related tweets from various twitter handles. Then the tweets are further filtered and only the required information from the tweets is extracted using spaCy and statistical modelling. This repo is created for trying out a basic NLP project of text classification using libraries like nltk,Spacy,numpy and sklearn.

You can test the implementation of the model hosted using flask at the following url https://tweeter-covid-filter.herokuapp.com/

ANI_Dataset.csv contains a collection of tweets scraped from ANI's tweeter feed and labelled based on the hashtags if it is a covid related news or not.

TwitterFeed.csv contains a collection of tweets which has been classfied and entities extracted from the tweets.


Purpose of files:
    1. CollectTweets.ipynb is used to gather the data from twitter and create the dataset with labels.
    2. TwitterModel.ipynb is used to do the statistical analysis, preprocessing and modelling of the dataset which has been generated using CollectTweets.py
    3. TweetContextExtraction.ipynb is used to extract the entitites from the predicted Covid related tweets by the model generated from TwitterModel.py.
    4. TwitterPredict.ipynb is used to for predicting any unkonwn tweets and extracting entities from it.

Generated Folder contains the different types models and functions like PCA, vectorizer etc generated during creating this model.


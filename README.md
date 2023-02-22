![header](./images/header.png)
# Overview

The goal of this project is to create and deploy a model that can predict the primary interest of a Twitter user between the following four interests using the user's most recent tweets and NLP/predictive machine learning: Sports / Entertainment, Politics, Science / Technology, and Business. Also, if the user's primary interest is politics, a secondary goal was to to predict the user's political affiliation.

The purpose of this classification system is more successful targeted advertising and for a more enjoyable user experience.

# Business Understanding 

The stakeholder is Twitter itself, and I'm illustrating to Twitter the ability to use NLP/predictive machine learning on a user's tweets to better segment its users for the purpose of targeted advertising.  Having the ability to identify the primary interest of a user is invaluable for segmentation / targeted advertising.

# Data Understanding
For this analysis, I utilized ~136K tweets pulled from 612 Twitter accounts by me from the Twitter API. These accounts were manually selected by me to represent each account class that I am trying to predict.

The model created for the classification of users into the four primary segments is known as model 1. For model 1, I scaled down the population of political tweets used to train the model to a smaller dataset and separate file consisting of ~101K tweets.

Model 2 representions the secondary classfication of political users between conservative and liberal classes. For this model, I utilized all tweets collected from political accounts.

# Exploratory Data Analysis


# Modeling
For both models, I used NLP techniques and a Complement Naive Bayes Classifier to predict the primary interest of the user between the four categories and then to predict the political affiliation of political users.  The first step is preprocessing the tweets using NLTK, which includes tokenizing the tweets using a regular expression tokenizer, removing stop words, and stemming the words. This preprocessing step is performed on the 'tweet' column of the data and the result is stored in a new column 'preprocessed_tweet'.
. I performed some manual preprocessing, then used a TFIDF vectorizor, then used a Complement Naive Bayes Classifier to fit the training data and predict the primary interest of the user and/or political affiliation.  
# Final Evaluation

# Next Steps
Recommendation to Twitter for next steps: 
- Deploy the model at Twitter to better segment its users and improve targeted advertising.
- Run the model routinely on all its users, as interests change with people over time.

## For More Information   

See the full analysis in the [Jupyter Notebook](./notebook_01_main.ipynb) or review this [presentation](./presentation.pdf).

**For additional info, contact:**
- Nate Kist: natekist@outlook.com

## Repository Structure

```
├── images
│   ├── slides_header.jpg
│   ├── negative_words.png
│   ├── positive_words.png
│   ├── product_sentiment.png
│   ├── tweets_by_company.png
├── data
│   ├── judge-1377884607_tweet_product_company.csv
├── eda_notebooks
│   ├── index_Nate - v3.ipynb.csv
│   ├── index_just_eda_zach.ipynb
├── notebook.ipynb
├── presentation.pdf
└── README.md
```




# Twitter Sentiment Analysis

## Introduction
This project focuses on performing sentiment analysis on Twitter data using machine learning techniques. It aims to classify tweets as either positive or negative sentiment based on their textual content. The project utilizes a dataset of tweets and applies natural language processing and machine learning models to make sentiment predictions.

## Prerequisites
Before running the code, ensure you have the following libraries and tools installed:
- Python 3.x
- Jupyter Notebook or any Python IDE
- Required Python libraries (NumPy, Pandas, Seaborn, Matplotlib, NLTK, Scikit-learn, WordCloud)

## Dataset
The dataset used in this project is sourced from a CSV file named `training.1600000.processed.noemoticon.csv`. It contains the following columns:
- target: Sentiment label (0 for negative, 4 for positive)
- ids: Tweet ID
- date: Date of the tweet
- flag: Flag (not used in this analysis)
- user: User who posted the tweet
- text: The tweet's text content

## Data Preprocessing
- The dataset is loaded and columns irrelevant to sentiment analysis are removed.
- Text preprocessing includes cleaning, lemmatization, and replacing URLs, emojis, and mentions with placeholders.
- Stop words are removed, and text data is tokenized.

## Exploratory Data Analysis (EDA)
- EDA is performed to visualize the distribution of sentiment labels in the dataset.
- Word clouds are generated to visualize the most frequent words in positive and negative tweets.

## Model Building
Three machine learning models are trained and evaluated for sentiment classification:
1. Logistic Regression
2. Linear Support Vector Classifier (LinearSVC)
3. Bernoulli Naive Bayes (BernoulliNB)

## Model Evaluation
- Model performance metrics such as precision, recall, F1-score, and confusion matrices are displayed for each model.
- Logistic Regression demonstrates the best performance with an accuracy of approximately 82%.

## Saving Models
The trained models (vectorizer, Logistic Regression, and BernoulliNB) are saved using pickle for future use.

## Predicting Sentiments
A script is provided to predict the sentiments of user-provided tweets using the trained Logistic Regression model.

## Usage
1. Install the required libraries mentioned in the Prerequisites section.
2. Run the Jupyter Notebook or Python script to execute the entire analysis.
3. Use the provided script to predict the sentiment of user-provided tweets.







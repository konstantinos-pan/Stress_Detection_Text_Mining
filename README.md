# Stress Detection Text Mining
This machine-learning project objective is to detect stress from social media articles and is co-autored by **Panagiotis Makropoulos**. The dataset used is publicly available at Kaggle ([Stress Detection from Social Media Articles](https://www.kaggle.com/datasets/mexwell/stress-detection-from-social-media-articles)). On this project we used *"Twitter_Full.csv"* file that contains Tweeter posts from September 2019 to September 2021.

# 1. Data Preprocessing - Feature Extraction
After performing exploratory data analysis and data visualization data preprocessing techinques for text data were used. Specifically, we removed duplicates and null values, removed text noise (urls, html tags, punctuation, stopwords) and performed lemmatization utilizing WordNet Lemmatizer. In order to extract features from text data we used Word2Vec word embedding technique and experimented with two different approaches. The first approach was to train a Word2Vec model on the training dataset corpus and the second one was to load the pre-trained Word2Vec model *"word2vec-google-news-300"* which was trained on a exceptionally larger corpus from Google News articles. In both cases, Principal Component Analysis was performed in order to reduce data dimensionality.

# 2. Methodology

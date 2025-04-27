# Yelp Reviews Classification

## Problem Statement
The project aims to classify Yelp reviews into positive or negative categories using Natural Language Processing (NLP) techniques.

## EDA (Exploratory Data Analysis)
### Data Cleaning steps:
- Removing punctuation: manually defined a function to remove punctuation.
- Removing stopwords: used nltk.corpus.stopwords.
- Tokenization: splitting sentences into words.
  
### Feature Engineering
- Count Vectorization: Used CountVectorizer from scikit-learn.
- Converted text into a bag-of-words representation.
- Later, TF-IDF Transformation was applied:
- Used TfidfTransformer after CountVectorizer to enhance the model.

## Model Building and Training
### First model:
- Algorithm: Multinomial Naive Bayes (MultinomialNB)
- Trained on Count Vectorized data.

### Second model (after feature enhancement):
- Added TF-IDF features on top of Count Vectorized data.
- Again used MultinomialNB.

### Summary of First Model :
- Accuracy: 0.92 (from average of the precision and recall)
- Precision (Weighted): 0.92
- Recall (Weighted): 0.92
- F1-score (Weighted): 0.91

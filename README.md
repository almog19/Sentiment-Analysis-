# Sentiment-Analysis-
This repository contains a learning and testing process of supervised machine learning model for sentiment analysis classifiers which has tested many ways to achieve different results, which get input sentences and categorize them into three categories: 
- Positive
- Negative
- Neutral 
The project demonstrates end-to-end Natural Language Processing (NLP) workflow development, including data preprocessing, feature engineering, model training, evaluation, and deployment-ready inference.
the purpsoe of the model is to understand of the words base on their absolute meaning, and their meaning base on the context.
for example:
good -> possitive
not good -> negative
##techniques used:
1) NLP Preprocessing: tokenization, stopword removal(in some models), lemmatization .
2) Feature Extraction: TF-IDF, word embeddings (implemented both, word embedding has achieved better results).
3) Modeling: neural network classifier (embedding layer, biLSTM).
4) Evaluation: Accuracy, precision, recall, F1-Score, and confusion matrix.
5) Production-Ready: Includes a standalone prediction script for easy deployment or integration into applications.

##Data Set
the used dataset is a collection of labeled tweets, including slang word

## preprocessing

    1) clean the text
        - lowercasing
        - remove links and useranames
        - reduce reapted letters (soo -> so)
        - remove special character and letters
        - remove extra spaces
        - split the sentence into words
        - lemmatize(going -> go, better -> well, teeth -> tooth)
    2) tokenization and sequencing
        - associate a word(text) to a value(token) base on a vocabulary
        - pad the sequence into a single input length
    3) features engeneering
        a layer that will give a value of a vector(d dimentions), each demention determine the similarity or disimilarity of the word(work like an attention layer)


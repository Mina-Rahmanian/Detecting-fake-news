# Detecting-Fake-News
<br /><br />
## Introduction

Fake news is false information and hoaxes spread through social media and other online media to achieve a political agenda. In this data science project idea, we will use Python to build a model that can accurately detect whether a piece of news is real or fake. We’ll build a TfidfVectorizer and use a PassiveAggressiveClassifier to classify news into “Real” and “Fake”. We’ll be using a dataset of shape 7796×4 and execute everything in Jupyter Lab.

Language: Python <br />
Dataset/Package: [news.csv](https://github.com/Mina-Rahmanian/Detecting-fake-news/blob/main/news.csv)

----------------------------------------------------------------------------------------------------
The main goal of this challenge is to To build a model to accurately classify a piece of news as REAL or FAKE spread through online media.
<br /><br />

<p align="center">
<img width="750" height="400" alt="d1" src="https://user-images.githubusercontent.com/71558720/195906991-db366e95-8769-4c6d-af5e-50ef819be7ec.PNG">
</p>
<p align="center">
<em>Fig.1: Detecting Fake News</em>
</p> <br /> 


## What is a TfidfVectorizer?

**TF (Term Frequency):** The number of times a word appears in a document is its Term Frequency. A higher value means a term appears more often than others, and so, the document is a good match when the term is part of the search terms.

**IDF (Inverse Document Frequency):** Words that occur many times a document, but also occur many times in many others, may be irrelevant. IDF is a measure of how significant a term is in the entire corpus.

The TfidfVectorizer converts a collection of raw documents into a matrix of TF-IDF features. Let’s initialize a [TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html) with stop words from the English language and a maximum document frequency of 0.7 (terms with a higher document frequency will be discarded). Stop words are the most common words in a language that are to be filtered out before processing the natural language data. And a TfidfVectorizer turns a collection of raw documents into a matrix of TF-IDF features.


## What is a PassiveAggressiveClassifier?

**Passive Aggressive algorithms** are online learning algorithms. Such an algorithm remains passive for a correct classification outcome, and turns aggressive in the event of a miscalculation, updating and adjusting. Unlike most other algorithms, it does not converge. Its purpose is to make updates that correct the loss, causing very little change in the norm of the weight vector.

----------------------------------------------------------------------------------------------------
## Summery of the Project

This project of detecting fake news deals with fake and real news. Using **sklearn**, we build a TfidfVectorizer on our dataset. Then, we initialize a PassiveAggressive Classifier and fit the model. In the end, the accuracy score and the confusion matrix tell us how well 


**Steps for detecting fake news with Python:** 

1) Install the following libraries with pip and make necessary imports

|pip install numpy pandas sklearn                                 | 
|:----------------------------------------------------------------|
|import numpy as np                                              |
|import pandas as pd                                             |
|import itertools                                                |
|from sklearn.model_selection import train_test_split            |
|from sklearn.feature_extraction.text import TfidfVectorizer     |
|from sklearn.linear_model import PassiveAggressiveClassifier    |
|from sklearn.metrics import accuracy_score, confusion_matrix    |   

2) let’s read the data into a DataFrame, and get the shape of the data and the first 10 records.
<br />
<p align="left">
<img width="750" height="300" alt="d1" src="https://user-images.githubusercontent.com/71558720/196262502-b9bcb683-e63f-4a31-9387-23bb518b68b0.PNG">
</p><br /> 

3) Get the labels from the DataFrame.

<p align="left">
<img width="170" height="200" alt="d1" src="https://user-images.githubusercontent.com/71558720/196262505-3e6b9e9e-7e07-4331-b191-094b490629fa.PNG">
</p><br /> 
4) Split the dataset into training and testing sets.

<br /><p align="left">
<img width="670" height="90" alt="d1" src="https://user-images.githubusercontent.com/71558720/196262506-37935b30-5d32-418a-a6e0-bfc067d7e6fc.PNG">
</p><br /> 
5) Fit and transform the vectorizer on the train set, and transform the vectorizer on the test set.

<br /><p align="left">
<img width="670" height="100" alt="d1" src="https://user-images.githubusercontent.com/71558720/196262516-6abaa673-92d8-4629-be80-06795f2c301b.PNG">
</p><br /> 
6) Initialize a PassiveAggressiveClassifier. This is. We’ll fit this on tfidf_train and y_train.<br /> 
7) predict on the test set from the TfidfVectorizer and calculate the accuracy with accuracy_score() from sklearn.metrics.<br /> 
8) We got an accuracy of 92.98% with this model. 

<br /><p align="left">
<img width="650" height="190" alt="d1" src="https://user-images.githubusercontent.com/71558720/196262517-147b4936-3971-492b-bd2d-40f623f534ef.PNG">
</p><br /> 
9) Finally, let’s print out a confusion matrix to gain insight into the number of false and true negatives and positives.

<p align="left">
<img width="85" height="80" alt="d1" src="https://user-images.githubusercontent.com/71558720/196262500-9a243a64-d343-4b8e-a7cc-3c11b34d5a2a.PNG">
</p><br /> 
10) Perfect we have done :)

<p align="center">
<img width="500" height="110" alt="d1" src="https://user-images.githubusercontent.com/71558720/196265058-9f0b3a59-32d7-4a3f-8729-3df9b3b8cb54.png">
</p><br /> 
 In this model, we have 589 true positives, 587 true negatives, 42 false positives, and 49 false negatives.


## Conclusion


Today, you have learned to detect fake news with Python. We took a political dataset, implemented a TfidfVectorizer, initialized a PassiveAggressiveClassifier, and fit our model. We ended up obtaining an accuracy of 92.98% in magnitude.

Hope you enjoyed the fake news detection python project.
<br /> <br /> 
 
 
 
 
## ** Mina R **



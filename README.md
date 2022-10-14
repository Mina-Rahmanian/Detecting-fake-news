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


###Steps for detecting fake news with Python





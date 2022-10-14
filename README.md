# Detecting-Fake-News
<br /><br />
## Introduction

Fake news is false information and hoaxes spread through social media and other online media to achieve a political agenda. In this data science project idea, we will use Python to build a model that can accurately detect whether a piece of news is real or fake. We’ll build a TfidfVectorizer and use a PassiveAggressiveClassifier to classify news into “Real” and “Fake”. We’ll be using a dataset of shape 7796×4 and execute everything in Jupyter Lab.

Language: Python <br />
Dataset/Package: [news.csv](https://github.com/Mina-Rahmanian/Detecting-fake-news/blob/main/news.csv)

----------------------------------------------------------------------------------------------------
The main goal of this challenge is to detect fake and real news that is generally spread through social media and other online media.
<br /><br />

<p align="center">
<img width="750" height="400" alt="d1" src="https://user-images.githubusercontent.com/71558720/195906991-db366e95-8769-4c6d-af5e-50ef819be7ec.PNG">
</p>
<p align="center">
<em>Fig.1: Detecting Fake News</em>
</p> <br /> 


## What is a TfidfVectorizer?
<br />
**TF (Term Frequency):** The number of times a word appears in a document is its Term Frequency. A higher value means a term appears more often than others, and so, the document is a good match when the term is part of the search terms.

**IDF (Inverse Document Frequency):** Words that occur many times a document, but also occur many times in many others, may be irrelevant. IDF is a measure of how significant a term is in the entire corpus.

The TfidfVectorizer converts a collection of raw documents into a matrix of TF-IDF features.

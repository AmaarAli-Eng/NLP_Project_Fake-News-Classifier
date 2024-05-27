# Fake News Classifier

This project implements a fake news classifier using machine learning techniques. The classifier is built using Python and various libraries such as `nltk`, `pandas`, `scikit-learn`, and more.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)

## Introduction

The goal of this project is to classify news articles as either fake or real. This is achieved by training a machine learning model on a labeled dataset of news articles. The classifier preprocesses the text, extracts features using TF-IDF, and then applies the model to predict the labels.

## Dataset

The datasets used in this project are `kaggle_fake_train.csv` and `kaggle_fake_test.csv`.

### Training Data (`kaggle_fake_train.csv`)
- `id`: Unique identifier for each news article.
- `title`: Title of the news article.
- `author`: Author of the news article.
- `text`: Full text of the news article.
- `label`: Binary label where `1` indicates fake news and `0` indicates real news.

### Testing Data (`kaggle_fake_test.csv`)
- `id`: Unique identifier for each news article.
- `title`: Title of the news article.
- `author`: Author of the news article.
- `text`: Full text of the news article.

## Dependencies

To run the code in this repository, you will need the following Python libraries:
- `nltk`
- `pandas`
- `numpy`
- `scikit-learn`
- `google-colab` (if using Google Colab)

You can install these dependencies using `pip`: pip install nltk pandas numpy scikit-learn

##  Model Training and Evaluation

The notebook performs the following steps:

- Connecting to Google Drive: (if using Google Colab)
- Text Preprocessing: Cleans the text by removing non-alphabet characters, converting to lowercase, lemmatizing, and removing stop words.
- Feature Extraction: Uses TfidfVectorizer to transform the processed text into TF-IDF features.
- Model Training: Trains a machine learning model on the training data.
- Evaluation: Evaluates the model using accuracy score, precision, recall, and F1-score.


##Results

After running the notebook, you will see various evaluation metrics printed in the output, indicating the performance of the fake news classifier on the dataset.

# Mental Disorder Detection Model for Egyptian Arabic Dialect

## Table of Contents

  - [Introduction](#introduction)
  - [Documentation](#documentation)
  - [Methodology](#methodology) 
  - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
  - [Pre-processing](#pre-processing)
  - [Feature Engineering](#feature-engineering)
  - [Model Building](#model-building)
  - [Evaluation](#evaluation)
  - [Prediction](#prediction)
  - [Model Saving](#model-saving)
    
## Introduction

This machine-learning model is intended to detect Depression, anxiety, and suicidal thoughts using textual data. It uses natural language processing (NLP) techniques and machine learning algorithms to classify input text into one of three categories: depression, anxiety, or suicidal tendencies. We manually acquired our dataset from Reddit, Sanvello, Twitter, Happify, and Facebook, which included posts from people suffering from mental disorders. Some records are in the Egyptian dialect of Arabic, while others are in English, which we translated and converted to Egyptian Arabic. It contains 1800 records, including 600 for depression, 600 for anxiety, and 600 for suicidal tendencies.

## Documentation

[Documentation](https://drive.google.com/file/d/1zV7Fo9f53qx_AvW17I9bnM_hE6i3JwnH/view?usp=sharing)

## Methodology
  ### Exploratory Data Analysis (EDA)

The model includes an initial exploratory data analysis (EDA) phase to understand the dataset's characteristics, such as data distribution, missing values, and data insights.

  ### Pre-processing

The textual data undergoes several pre-processing steps, including:
- HTML tag removal
- Arabic diacritics removal
- Punctuation removal
- Stopword removal
- Stemming
- Emoji removal

### Feature Engineering

Feature engineering involves creating bag-of-words (BOW), TF-IDF, and Word2Vec representations of the text data to extract meaningful features for model training.

  ### Model Building

The model utilizes various machine learning algorithms, including:
- K Nearest Neighbors
- Decision Tree
- Random Forest
- Logistic Regression
- Naive Bayes
- Support Vector Machine (SVM)

Models are trained using both BOW, TF-IDF, and Word2Vec representations to compare performance across different feature extraction techniques.

  ### Evaluation

Model performance is evaluated using metrics such as accuracy, ROC-AUC, and classification reports. Cross-validation is employed to ensure robust evaluation.

  ### Prediction

The model provides predictions for input text data, categorizing it into depression, anxiety, suicidal tendencies, or other mental health categories based on learned patterns from the training data.

  ### Model Saving

Trained models are saved using joblib and pickle libraries for future use or integration into other applications.


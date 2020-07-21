# Authorship Profiling: Tweet Gender Classification

Foobar is a Python library for dealing with word pluralization.

## Description

These files generate the preprocessing and modelling for gender classification of tweets for a Monash Kaggle competition. The best model we were able to train was the Logistic Regression in `final_classifier.ipynb`.
![Imgur](https://i.imgur.com/ngPhkga.png)

## Files

This project comprises three Python3 Jupyter Notebook files:

   1. `data_wrangling`.ipynb
   2. `all_classifiers.ipynb`
   3. `final_classifier`.ipynb

Two .csv:

   1. `train_labels.csv`
   2. `test_labels.csv`

One ZIP file with the tweets.


## Usage

### Logistic Regression Test Predictions

To simply generate the final pred labels.csv, where the label prediction on the testing documents is stored, you can run the group41_ass2_final_classifier.ipynb file, which will be using train_labels.csv, bw_train.npy, bw_test.npy and test_index_list.npy to train and test the best selected model (Logistic Regression).

### Data Preparation & Feature Extration

To analyse the pre-processing steps, please open group41_ass2_wrangling.ipynb. It will go the data reading, preparation and feature extraction. The final method used for the modelling part was “CountVectorizer” with words and characters n-grams model. This is what generates bw_train.npy and bw_test.npy, which are the necessary files to run the top selected model. In order to run this file from the scratch, you need to add the data folder containing the unzipped data.zip contents in the same folder as you have the codes.

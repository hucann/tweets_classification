# Project Overview

This repository contains the code and data files for CS433 Machine Learning Project 2, which aims at predicting whether a smiley ":)" or sad ":(" emoji was originally present in a list of tweets.

## Usage Instructions

1. **Data Placement**:
   Place the data in the following structure:

   - **twitter-datasets/**
     - `test_data.txt`
     - `train_neg_full.txt`
     - `train_pos_full.txt`

2. **Generate trimmed training data**:
   Run `remove_duplicate.sh` on `train_neg_full.txt` and `train_pos_full.txt` to generate `train_neg_trimmed.txt` and `train_pos_trimmed.txt` respectively. Place the trimmed txt files in the same directory as above

3. **Generate Prediction**:
   Run xxxxx

## Files and Scripts

### ML Methods Implementations

- **`Model versions/`**: Contains implementations of multiple different variants of machine learning models implemented.
  - `Glove_embedding.ipynb`: Implementation of classical machine learning methods including logistic regression, SVM, and random forest using GloVe embeddings.
  - `LSTM_pytorch_without_paranthesis_detection.ipynb`: Implementation of LSTM model without custom features.
  - `LSTM_pytorch_with_paranthesis_detection.ipynb`: Implementation of LSTM model with custom features.
  - `BERT.ipynb`: Implementation of DistillBERT and DistillBERT.
  - smth abt auto regressor
  - `Bracket_matching.ipynb`: Result of purely using unbalanced parentheses method to predict the presence of smiley or sad emoji, with code to post-process predictions by detecting unbalanced parentheses. 


### Utilities

- **`utilities/`**: Contains utility functions and scripts to clean the data, and generate statistics. For example, it includes the scripts needed to generate GloVe embeddings, the script to remove duplicate tweets from training data and ipynb to generate statistics of unbalanced parentheses in the dataset.

### Additional Dataset

- **`additional-dataset/`**: **please insert**

### Model Prediction

- **`submission.pkl`**: Contains the final model predictions.
- **`run.py`**: Generates `submission.csv` by reading predictions from `submission.pkl`

## Libraries and packages used

Many external libraries and packages were used to help increase efficiency and accuracy of the models. The following is a list of the libraries and packages used in this project:

- **`pandas`**: Used for data manipulation and analysis.
- **`numpy`**: Used for numerical operations.
- **`pytorch`**: Used for building and training neural networks.
- **`sklearn`**: Used for machine learning models.
- **`transformers`**: Used for easily loading pre-trained models like BERT.

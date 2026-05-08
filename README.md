# Sentiment-Analysis-of-Social-Media-Comments-using-BILSTM-and-GloVe-embedddings
BiLSTM sentiment classifier with GloVe embeddings | 3 classes (positive/negative/natural) | 78% accuracy | Python


## Overview

This project performs sentiment analysis on social media comments using a **Bidirectional LSTM (BiLSTM)** network. The model classifies comments into three categories: Positive, Negative, or Natural.

After hyperparameter tuning, the model achieved **78% validation accuracy**.

## Dataset

The links of Two datasets from Kaggle that were used:
https://www.kaggle.com/datasets/abhi8923shriv/sentiment-analysis-dataset
https://www.kaggle.com/datasets/pradeeshprabhakar/preprocessed-dataset-sentiment-analysis

The link of the GloVe vectors:
https://www.kaggle.com/datasets/rtatman/glove-global-vectors-for-word-representation


| Metric | Value |
|--------|-------|
| Total unique records | 28,673 |
| Total unique words | 10,000 |
| GloVe vectors used | 400,000 |
| Final embedded vectors | 8,677 |

## Model Architecture

- **BiLSTM** – captures context from past and future time steps
- **GloVe embeddings** – pre-trained word vectors (400k vectors)

## EDA & Preprocessing

**Visualizations:** Bar chart, box plot, correlation matrix, histogram plot

**Preprocessing steps:** Lowercasing, removing punctuation/stopwords, tokenization, padding

## Training Hyperparameters

| Parameter | Value |
|-----------|-------|
| Optimizer | Adam |
| Loss | Categorical Crossentropy |
| Batch size | 64|
| Epochs | 10 |
| Validation split | 20% |
| Max sequence length | 100 |

## Evaluation Metrics

Accuracy, precision, recall, F1-measure, confusion matrix, macro avg, weighted avg

**Final validation accuracy: 78%**

Run the `.ipynb` notebook in Jupyter/Colab; a detailed academic report covering the full project pipeline (model choice, visualization, preprocessing, results) is also included.

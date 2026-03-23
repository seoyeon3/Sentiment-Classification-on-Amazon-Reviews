# Amazon Review Sentiment Analysis using LSTM
## Problem Definition
Extracting sentiment from large-scale textual reviews is essential for understanding customer opinions and improving product quality. This project aims to build an LSTM-based model to classify 200,000 Amazon reviews as positive or negative, leveraging sequential patterns in text data.

## Project Workflow

1. Defined the sentiment classification task using Amazon review data, including both review text and titles  

2. Performed exploratory data analysis (EDA)  
   - Analyzed text and title length distributions  
   - Examined class balance and common word patterns  

3. Text Preprocessing  [![Notebook](https://img.shields.io/badge/Notebook-Data%20Preprocessing-blue)](https://github.com/seoyeon3/Sentiment-Classification-on-Amazon-Reviews/blob/main/datapreprocessing_with_2classes.ipynb)
   - Applied lemmatization to normalize words  
   - Removed noise, punctuation, and stopwords  
   - Trimmed text to reduce irrelevant tokens  
   - Applied padding to ensure uniform input length  

4. Model Development [![Notebook](https://img.shields.io/badge/Notebook-LSTM-blue)](https://github.com/seoyeon3/Sentiment-Classification-on-Amazon-Reviews/blob/main/MultilayeredLSTM_2classModel_with_trimming.ipynb) 
   - Built LSTM models to capture sequential dependencies in text data  
   - Trained separate models using review text only and title only  
   - Designed a multi-input architecture combining text and title representations  
   - Stacked LSTM layers to learn richer feature representations  

5. Model Evaluation  
   - Compared performance across text-only, title-only, and combined models  
   - Evaluated using accuracy and loss metrics  

6. Final Model Selection  
   - Selected the combined text + title LSTM model based on improved performance    

## Key Results
[![Report](https://img.shields.io/badge/Report-LSTM%20Model-blue)](https://github.com/seoyeon3/Sentiment-Classification-on-Amazon-Reviews/blob/main/LSTM%20Model%20Report.pdf)

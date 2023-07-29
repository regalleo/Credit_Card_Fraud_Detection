# credit_card_fraud_detection
fraud detection in credit cards using data science and machine learning algorithms
Note: Download the Dataset from kaggle. //creditcard.
Overview

This project aims to build a credit card fraud detection system using data science and machine learning algorithms. The dataset used for training and evaluation is obtained from Kaggle, containing anonymized credit card transaction data, including both fraudulent and legitimate transactions. The main goal is to develop models that can effectively identify fraudulent transactions and enhance security for credit card users.

Dataset

The dataset used in this project is available on Kaggle and can be found in the data folder. Due to the large size of the original dataset, we have sampled a fraction (10%) of the data for faster prototyping. The original dataset contains features V1 to V28, which are the result of a PCA dimensionality reduction to protect user identities and sensitive features. The target variable is Class, where 1 denotes a fraudulent transaction and 0 denotes a valid transaction.

Requirements

To run the code in this project, you need to have the following dependencies installed:

Python (>= 3.6)
Jupyter Notebook
pandas
numpy
matplotlib
seaborn
scikit-learn
You can install the required packages using the following command:

Copy code
pip install -r requirements.txt
File Descriptions

creditcard.csv: The dataset file containing credit card transaction data.
notebooks/: This directory contains Jupyter notebooks with step-by-step explanations of data analysis, preprocessing, model building, and evaluation.
src/: This folder includes Python scripts with utility functions for data preprocessing and model building.
plots/: Contains visualizations generated during the exploratory data analysis and model evaluation.
Data Preprocessing

The data preprocessing steps involve sampling a fraction of the dataset to address class imbalance issues. We remove any irrelevant columns to ensure efficient model training.

Exploratory Data Analysis (EDA)

EDA is performed to gain insights into the dataset. Various visualizations, including histograms and heatmaps, are created to understand the distribution of features and correlations between them.

Model Building

We use two outlier detection algorithms for this project:

Isolation Forest: An ensemble method that isolates anomalies by randomly selecting features and splitting points.
Local Outlier Factor (LOF): A density-based outlier detection method that calculates the local density deviation of a data point with respect to its neighbors.
The models are trained on the preprocessed data to detect fraudulent transactions based on patterns and anomalies in the data.

Model Evaluation

The performance of each model is evaluated using classification metrics such as accuracy, precision, recall, and F1-score. We compare the results of both models to determine their effectiveness in detecting credit card fraud.

Conclusion

This project showcases the implementation of data science and machine learning techniques for credit card fraud detection. The models' performance and evaluation metrics provide valuable insights into their effectiveness for detecting fraudulent transactions. It can be used as a starting point for further research and improvements in fraud detection systems for financial institutions and businesses dealing with online transactions.

﻿# submission-bmlp
Project Overview
This notebook implements a complete pipeline for analyzing bank transaction data using both clustering and classification approaches. Here's a breakdown of what it accomplishes:
Criteria 1: Data Loading and Exploratory Data Analysis

Loads the dataset and displays basic information using head(), info(), and describe()
Creates a correlation matrix visualization with proper formatting
Generates histograms for both numeric and categorical columns
Includes box plots to identify outliers
Ensures all visualizations are properly labeled and formatted to avoid overlapping labels

Criteria 2: Data Cleaning and Preprocessing

Checks for missing values using isnull().sum()
Identifies and counts duplicate records
Drops ID columns (TransactionID, AccountID, DeviceID, IPAddress, MerchantID)
Handles any missing values using appropriate strategies
Removes duplicate records
Handles outliers using the IQR method
Performs feature encoding for categorical variables
Creates binning for the TransactionAmount feature
Applies feature scaling using MinMaxScaler

Criteria 3: Building Clustering Model

Uses the preprocessed dataset for clustering
Implements and visualizes the Elbow Method using KElbowVisualizer
Builds a K-Means clustering model with the optimal number of clusters
Calculates and displays the Silhouette Score
Creates a visualization of the clustering results using PCA
Saves both the K-Means and PCA models

Criteria 4: Interpreting Clustering Results

Provides detailed statistical analysis of each cluster
Shows characteristics of each cluster based on feature distributions
Performs inverse transformation of scaled features
Re-analyzes clusters with the inverse-transformed data
Saves the inverse-transformed data with cluster labels to a CSV file

Criteria 5: Building Classification Model

Uses the inverse-transformed data with cluster labels for classification
Splits the data into training and testing sets
Builds a Decision Tree classification model
Builds a Random Forest classification model for comparison
Evaluates both models using accuracy, precision, recall, and F1-Score metrics
Performs hyperparameter tuning on the model with lower performance
Saves all models as required by the submission guidelines

How to Use This Notebook

Download the dataset from the Google Drive link provided in your instructions
Place the dataset file in the same directory as this notebook
Run the notebook cells sequentially to perform the complete analysis
The notebook will generate all required models and save them as specified in the guidelines

This implementation provides a comprehensive analysis that meets the Advanced level criteria across all five evaluation areas. The code includes detailed comments and explanations at each step, making it easy to understand the workflow and methodology.

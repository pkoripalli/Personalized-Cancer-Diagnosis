# Personalized Cancer Diagnosis

### Business Problem

### Description
Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/

Data: Memorial Sloan Kettering Cancer Center (MSKCC)

Download training_variants.zip and training_text.zip from Kaggle.

### Context:
Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/discussion/35336#198462

### Problem statement :
Classify the given genetic variations/mutations based on evidence from text-based clinical literature.

### Machine Learning Problem Formulation

### Data

### Data Overview

Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/data
We have two data files: one conatins the information about the genetic mutations and the other contains the clinical evidence (text) that human experts/pathologists use to classify the genetic mutations.
Both these data files are have a common column called ID

### Mapping the real-world problem to an ML problem

Objective: Predict the probability of each data-point belonging to each of the nine classes.

Constraints:

  Interpretability
  Class probabilities are needed.
  Penalize the errors in class probabilites => Metric is Log-loss.
  No Latency constraints.
  
### Train, CV and Test Datasets

Split the dataset randomly into three parts train, cross validation and test with 64%,16%, 20% of data respectively

### Exploratory Data Analysis

### Reading Data
### Reading Gene and Variation Data
### Reading Text Data
### Preprocessing of text
### Test, Train and Cross Validation Split
#### Splitting data into train, test and cross validation (64:20:16)
#### Distribution of y_i's in Train, Test and Cross Validation datasets

### Prediction using a 'Random' Model

In a 'Random' Model, we generate the NINE class probabilites randomly such that they sum to 1.

### Univariate Analysis

Univariate Analysis on Gene Feature
Univariate Analysis on Variation Feature
Univariate Analysis on Text Feature

### Machine Learning Models

Naive Bayes
K Nearest Neighbour Classification
Logistic Regression with Class balancing
Logistic Regression without Class balancing
Linear Support Vector Machines
Random Forest Classifier
Logistic regression with CountVectorizer Features, including both unigrams and bigrams
Performed Feature Engineering to improve the performance

### Conclusion

After some feature engineering we manage to decrease the log loss below < 1.

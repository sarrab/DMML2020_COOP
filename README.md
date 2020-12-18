# Data Mining and Machine Learning -Master in Information Systems-2020 – COOP

## Authors:
- Osman Gokturk
- Jessy Inaka
- Sarra Berich

Submission results
![Submission results](https://github.com/tograh/testrepository/3DTest.png 861)
## Folder Structure
1. documents
  1.1.submission csv files
  1.2. Some result files to save the resulting accuracies
  
2. codes
  - 2.1 EDA.ipynb : This notebook contains exploratory data analysis and the hyperlinks to other notebooks. We recommend starting from this file. 
  - 2.2 Classification_Models : this notebook come after the EDA one. It contain experimentation with all models that we tried.
  - 2.3 LR_Models : This model comes after EDA one. And it conatins only Logistic Regeression with raw and cleaned data and feature selection.
  - 2.4 Cleaning : It represents the deep cleaning that we performed at the end before applying our last model (last improvements).
  - 2.3 Last_Version : It represents our last version based on the conclusions retrieved form previous experiences. But, unfortunately the concurrence site was closed.
  
3. data:
  - 3.1 train_data
  - 3.2 test_data
  - 3.3 cleaned_data
## Video presentation

[![DMML2020 – Team COOP](")


## Table of Contents
1. Introduction
2. Methodology
3. Exploratory Data Analysis
4. Data Cleaning And Preprocessing
5. Feature Engineering
6. Models
7. Submissions


## 1. Introduction
### Real or Not? NLP with Disaster Tweets 
Text Analytics is one of the dynamic and frequently used field of Data Mining and Machine Learning. In this project we tried to make prediction based on a test data, which lack labels. We tried to guess correctly the labels as much as possible. 


## 2. Methodology
After defining several different data cleaner and preprocessing functions, we implemented for different type of models like: LogisticRegression, DecisionTreeClassifier, RandomForestClassifier, KNeighborsClassifier, Grid Search algorithm. We tried to observe the efficiency of these models under different data cleaner and preprocessing functions. One of the earlier conclusion was the fact that further cleaning like implementing stemming had a negatif effect on the result. Based on this finding, we tried to hyperparametrize under different models. 

However, one of our final conlcusion was the fact that data cleaning stage could matter a lot. 

### Aim
The aim of our project is to train and build Machine Learning models that are able predict whether a tweet about a disaster is real or not with an accuracy outperforming the base rate each time. In this order, our team envisions to explore various possibilities by tunning the parameters of the chosen models so that the best accuracy score will be achieved.

##  Import of Libraries
WE had imported the relevant libraries that we were using in the class over the weeks. In adition to frequent libraries like pandas, mathplot, scikit-learn we made use of re, nltk as well. 

## 3. Data Set and Exploratory Data Analysis
Data consist of two set of data. The first one is around 6.5K "Disaster Tweets" with the associated label, whether they indicate true or not true disasters. Apart from the text, tweet id, keyword and location. 

The second data set was a smaller data set which did not contain the label column. Predicting the label column was the job of the project. 

WE had explored the data to observe the initial visualizations. We run frequency bars, scatter plots and correlation matrices to observe the relationships. In fact there was no obvious pattern in the data. This made us conclude that a further text analytics could make better predictions. 

## 4. Data Cleaning and Preprocessing
We defined different cleaning and preprocessing functions to process the tweet texts. Upon initial observation we decided not to make stemming.

## 5.Feature Engineering And Feature Creation
Feature engineering playing a crucial role, this work focuses on it. All the parameters, namely text, location and keyword, are considered as important; hence, many of the models are built taking them all into account as predictors. Further, the analysis shows that the length of the word is equally important, our study captures it and thus creates a new feature named Average word length to be used as another predictor. Furthermore, with the explosion of dimensionality space after vectorization by TF_IDF, which this study mainly uses, Principal Component Anlysis is used to reduce the latter dimensionality.

## 6.Models
We had tryied different models to increase the test accuracy. We made use of LogisticRegression, DecisionTreeClassifier, RandomForestClassifier, KNeighborsClassifier to observe the test results. 

## 7. Submissions
We tried to explore models with parameters that would generate the highest accuracies. Then we fitted with the given data set where labes are known. After this, we run for the test data and made predictions to submitted.  





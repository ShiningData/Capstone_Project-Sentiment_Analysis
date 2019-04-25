# NLP Sentiment Analysis on Beauty Products

## Introduction
The company wants to develop a software tool that will identify the positive and negative words which customers use when they write reviews for the beauty products as their purchase inclination. For that, they gave their 9 years beauty products’ reviews between 2005-2014 and asked us to develop a model which will identify positive and negative words used in the reviews as a component of customer’s sentiment towards to the company’s beauty products. 

## Project Proposal 
The problem and approach to solve the problem in project proposal. You can click [here](https://github.com/ShiningData/Capstone_Project-Sentiment_Analysis/blob/master/Project_Proposal/Capstone%20Project%20Proposal.pdf) to reach it. 

## Data

The data is in Standford Analysis Project (SNAP) webpage. The original data was in a JSON format there. In order to analyze the data, I imported JSON package and decoded JSON file with using query in order to convert JSON file to csv file format. The original dataset for this project can be found [here](http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Beauty_10.json.gz)

## Data Wrangling
  Data insection and text preprocessing is completed in this section. It can found [here](https://github.com/ShiningData/Capstone_Project-Sentiment_Analysis/blob/master/Data_Wrangling/Amazon_Beauty_Products_Review-Sentiment_Analysis.ipynb)

## Exploratory Data Analysis
Univarate and bivariate analysises are done by using bar charts and wordcloud visualizations. These analysis can be found [here](https://github.com/ShiningData/Capstone_Project-Sentiment_Analysis/blob/master/Data_Storytelling/Sentiment_Analysis_Data_Storytelling.ipynb)

## Modeling
This is a supervised binary classification problem. We are trying to predict the sentiment based on the reviews left by females who bought beauty products in Amazon e-commerce online platform. We used Python’s Scikit Learn libraries to solve the problem. In this context, we implemented Logistic Regression, Random Forest, Naive Bayes, XGBOOST, CatBoost algorithms and Simple Neural Network as well. 
Since the ratings of the reviews were not distributed normally, we decided to decrease rating classes from 5 to 2 by merging Rating 1-2 as ‘Bad’ and Rating 4-5 as 'Good' while dropping Rating 3 from the dataset.
For feature selection, we applied threshold for word occurrence with using min_df/max_df, PCA and Singular Value Decomposition. For feature engineering, we applied CountVectorizer, TF-IDF, Hashing Vectorizer and Word2Vec to the text data in order to turn a collection of text documents into numerical feature vectors. 

Modeling notebooks can be reached from following links. 

- [Count Vectorizer, TF-IDF, Hashing Vectorizer with Traditional Algorithms](https://github.com/ShiningData/Capstone_Project-Sentiment_Analysis/blob/master/Deliverables/Sentiment_Analysis-1_CV-TF_IDF-HASH.ipynb)
- [Threshold for word occurence, PCA, Singular Value Decomposition, SMOTE techniques used with Traditional Algorithms](https://github.com/ShiningData/Capstone_Project-Sentiment_Analysis/blob/master/Deliverables/Sentiment_Analysis-2_EXPWORDLST-SMOTE-PCA-TRNCTDSVD.ipynb)
- [Word2Vec with Keras](https://github.com/ShiningData/Capstone_Project-Sentiment_Analysis/blob/master/Deliverables/Sentiment_Analysis-3_Word2Vec-Keras.ipynb)

##



The original dataset for this project can be found (here)[https://www.kaggle.com/uciml/default-of-credit-card-clients-dataset/home The paper referenced in this project can be found here: https://bradzzz.gitbooks.io/ga-dsi-seattle/content/dsi/dsi_05_classification_databases/2.1-lesson/assets/datasets/DefaultCreditCardClients_yeh_2009.pdf]

The order for this project is as follows:

Project Proposal: https://github.com/gblinick/Springboard-Capstone-1/tree/master/Project%20Proposal
Data Wrangling: https://github.com/gblinick/Springboard-Capstone-1/tree/master/Data%20Wrangling
EDA: https://github.com/gblinick/Springboard-Capstone-1/tree/master/EDA
Inferential Statistics: https://github.com/gblinick/Springboard-Capstone-1/tree/master/Inferential%20Statistics
Milestone Report: https://github.com/gblinick/Springboard-Capstone-1/tree/master/Milestone%20Report
In-depth Analysis (Machine Learning): https://github.com/gblinick/Springboard-Capstone-1/tree/master/In-depth%20analysis
Final Report: https://github.com/gblinick/Springboard-Capstone-1/tree/master/Final%20Report
The most important files are:

Project Presentation: https://github.com/gblinick/Springboard-Capstone-1/blob/master/Final%20Report/Predicting%20Credit%20Card%20Default%20with%20scikit-learn.pdf
Project Report: https://github.com/gblinick/Springboard-Capstone-1/blob/master/Final%20Report/Final%20Report.pdf
In-depth Analysis Notebook: https://github.com/gblinick/Springboard-Capstone-1/blob/master/In-depth%20analysis/In-depth%20Analysis.ipynb

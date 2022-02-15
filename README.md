# spark_to_sparkify
The code for Udacity NanoDegree capstone project :

# Background and motivation
Sparkify is a music streaming simulation platform built by Udacity. Through this project, this platform's log data is provided to gain insights and develop a machine learning pipeline to predict churn. Users can listen to music for free (with ads between songs) or for a flat fee. They can upgrade, downgrade or cancel their subscription. The goal is to predict the user who will quit so as to offer him/her a significant discount before cancelling his/her subscription. User churn is a general problem that is extremely relevant and common in the industry. Recently, big data technologies offer a good solution to avoid user churn by providing relevant information to predict future customer behavior. That's why I chose this project that allows learning Spark, one of the most used big data technologies.

# Environement

* Anaconda 3
* Python 3.7.3
* pyspark 2.4
* pyspark.ml
* pandas

# Dataset

* mini_sparkify_event_data.json is the mini data that you can play with it to create your spark pipeline.

# Results

After exploring the data and creating relevent features Three classifiers re used to predict the user churn (binary prediction):
* Logistic regression
* Random Forest
* Decision trees

Models are tuned using gridsearch strategy with two paramters for each model and  CV folds. Results of the three models on the small data set are as follow:


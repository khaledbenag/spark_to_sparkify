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

After exploring the data and creating relevent features Three classifiers re used to predict the user churn (binary prediction). Models are tuned using gridsearch strategy with two paramters for each model and  CV folds. Results of the three models on the small data set are as follow::

* Logistic regression
  - Baseline: 
     ** The F1 score on the test set is 80.65%
     ** The areaUnderROC on the test set is 92.00%
  - Params tuning:
     ** The F1 score on the test set is 92.00%
     ** The areaUnderROC on the test set is 93.00%
* Random Forest
  - Baseline: 
     ** The F1 score on the test set is 82.38%
     ** The areaUnderROC on the test set is 75.00%
  - Params tuning:
     ** The F1 score on the test set is 76.41%
     ** The areaUnderROC on the test set is 85.00%
* Decision trees
  - Baseline: 
     ** The F1 score on the test set is 88.39%
     ** The areaUnderROC on the test set is 84.00%
  - Params tuning:
     ** The F1 score on the test set is 88.90%
     ** The areaUnderROC on the test set is 94.50%




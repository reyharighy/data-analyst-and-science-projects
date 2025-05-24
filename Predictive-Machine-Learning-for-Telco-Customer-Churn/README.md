# Predictive Machine Learning for Telco Customer Churn
![Project Logo](banner.jpg)

## Background
Currently, telecommunications service customers have numerous options and can easily switch subscriptions from one service provider to another. Marketing practitioners in this industry strive to prevent customers from switching to competing companies. Why is that? Because acquiring new customers is far more expensive than retaining loyal existing customers. Therefore, retaining existing customers is a high priority compared to acquiring new customers.

A common approach is to provide special pricing packages or bonuses to customers to prevent them from being tempted to switch to a competing company. However, if such offers are extended to all existing customers, the cost can become expensive as only a small fraction of customers tend to churn (unsubscribe) in general. A more effective approach is to ensure that special offers or bonuses are only given to specific customers known to have a propensity to churn.

## Table of Contents
- [Case Analysis and Goals](#case-analysis-and-goals)
- [Data Understanding](#data-understanding)
- [Explanatory Data Analysis](#explanatory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Model Benchmarking](#model-benchmarking)
- [Imbalanced Dataset](#imbalanced-dataset)
- [Hyperparameter Tuning](#hyperparameter-tuning)
- [Model Explanation](#model-explanation)

## Case Analysis and Goals
In this case, a predictive model will be developed for a telecommunications company with promotional programs that will only be offered to a group of customers deemed susceptible to churn. To make this more effective, Machine Learning is required to identify this customer group. The goal of this predictive model is to generate a churn score for each customer, indicating whether they are predicted to unsubscribe or not. This predictive model will use predictors based on patterns of customer internet service usage on the company's network.

How can the created prediction discern customer usage patterns? An individual's past behavior can serve as a reference point for understanding their future behavior. These behaviors are what will be analyzed from the available data. By identifying the signs that indicate someone is likely to churn, the company can take measures to prevent them from actually unsubscribing.

## Data Understanding
At this stage, Data Understanding is performed with the aim of gaining a deeper understanding of the data characteristics being analyzed before getting into Explanatory Data Analysis. Some steps of preparation are conducted as a slight cleanse process, those are data formatting and duplicates. Futher preparation processes will go along with in Explanatory Data Analysis. Please find the detailed process in [Data Understanding](Data_Understanding.ipynb).

## Explanatory Data Analysis
Explanatory Data Analysis is very critical before building a predictive model. This includes identifying patterns, trends, relationships, anomalies in data, as well as revealing insights that may not be visible directly. As for visualization, we will use library from **Matplotlib** and **Seaborn**. Please find the detailed process in [Explanatory Data Analysis](Explanatory_Data_Analysis.ipynb).

## Feature Engineering
Before doing machine learning modeling, a process is needed to prepare the raw data into ready-to-use data. In other words, this process is referred to as feature engineering. By doing good feature engineering, machine learning models can provide more accurate and better results in predicting target variables. Please find the detailed process in [Feature Engineering](Feature_Engineering.ipynb).

## Model Benchmarking
At this stage, the process of evaluating the performance of various machine learning model algorithms will be carried out by testing each model using various subsets of the available data and calculating the average score used as a reference for the assessment. This method is used to provide a more reliable and accurate estimate of the performance of each machine learning model when faced with new data sets. Please find the detailed process in [Model Benchmarking](Model_Benchmarking.ipynb).

## Imbalanced Dataset
The dataset as a whole has an unequal proportion of target classes where in this case study, the number of customers who churn is far less than subscribers who are still subscribed. This can cause several disadvantages, including model performance that tends to be biased, poor generalization, non-representative measurement evaluation results, and wrong interpretation of existing problems. This happens because the amount of data for the minority class, in this case churn customers, is insufficient when the training process is carried out on the algorithm model used. As a result, the algorithm model will produce poor performance in detecting churn customers even though overall it has fairly good accuracy. These deficiencies can be anticipated by manipulating the data so that the number of positive and negative classes is equal. Please find the detailed process in [Imbalanced Dataset](Imbalanced_Dataset.ipynb).

## Hyperparameter Tuning
Basically the developed algorithm model can produce more optimal performance by adjusting a set of hyperparameters from the algorithm model itself. The goal of hyperparameter tuning is to find the combination of parameters that produces the best model performance, including searching through hyperparameter tuning to find optimal values ​​based on certain evaluation metrics. Please find the detailed process in [Hyperparameter Tuning](Hyperparameter_Tuning.ipynb).

## Model Explanation
Model explanation refers to the process of understanding and explaining how the algorithm model works in making predictions. The goal is to provide insights and find out what factors contribute to the output produced. In this case, a number of features are provided from past data regarding customer information using the company's services and labels that reflect the subscription status of each customer. The company wants to know what factors cause a customer to churn and evaluate existing business models with the aim that customer retention can be as high as possible. In this section, we also include the conclusion and recommendations to apply for company's business development based on classification model established. Please find the detailed process in [Model Explanation](Model_Explanation.ipynb).

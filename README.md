# loan-pred-customer-behavior
Predict who possible Defaulters are for the Consumer Loans Product

# Dataset Introduction

This dataset belongs to a Hackathon organized by "Univ.AI". The dataset contains information about histoic customer behaviors observed by an organization, including income, age, experience, profession, married, house ownership, car ownership, risk flag, state, city, current house years and current job years. There are 13 variables in this dataset, whose length is 252k.

# Problem Statement

An organization wants to predict who possible defaulters are for the consumer loans product. They have data about historic customer behavior based on what they have observed. Hence when they acquire new customers they want to predict who is riskier and who is not. In this project, I am going to build and optimize some models from both supervised and unsupervised learning perspectives in order to achieve better predictive performance.

## Supervised Learning Outline

As mentioned before, our goal is to build a model to predict whether a customer is a riskier or not. This kind of prediction makes great sense in terms of new customer detection and risk assessment of existing users. Such algorithm design is part of responsibility of risk management, which is an extremely important part in most business companies.

Based on this, I will use the following outline for the design and implementation of the supervised section:

- Feature engineering, including data pre-processing, feature selection and so on.
- Model building, evaluation, slection and explanation.

**I intend to extract the data pre-processing part separately before all modeling work, because both supervised and unsupervised learning need to use that reasonably processed dataset.**

## Unsupervised Learning Synopsis

Based on the fact that we can build a reasonable model to predict the riskier among customer via supervised learning I dicussed above, here we apply unsuperivised learning to check whether feature extraction can improve the model performance. On the other hand, customer group segmentation based on some customers' features can help the bussiness stakeholds know guest better and faster, thus maximizing the bussiness benefits and minimizing the loss caused by riskiers. Therefore, what I want to deliver in this part are as following:

- Explore dimensionality reduction effect on the classification model performance improvement.
- Make customer group segmentation based on clustering algorithm.

# Development environment and dependencies

- Dataset: This dataset can be downloaded from [kaggle](https://www.kaggle.com/subhamjain/loan-prediction-based-on-customer-behavior/download). In addition, to facilitate version maintenance and dataset recall, the project is backed up on [github](https://github.com/shimmerjordan/loan-pred-customer-behavior) and the project reads the csv dataset from [github](https://github.com/shimmerjordan/loan-pred-customer-behavior/tree/main/data) by default.
- Runtime: Developed and debugged on [colab](https://colab.research.google.com/drive/13NRJMpuXKwzEEb_AJKZEpGjrGxtuTwSA?usp=sharing); (You can view, comment and run via this link, but without editing for security)
- Dependencies and packages:
  - imbalanced_learn==0.8.1
  - imblearn==0.0
  - keras==2.6.0
  - matplotlib==3.4.3
  - numpy==1.19.5
  - pandas==1.3.2
  - plotly==5.3.1
  - scikit_learn==1.0.1
  - seaborn==0.11.2
  - tensorflow==2.6.0
  - xgboost==1.5.0
  - yellowbrick==1.3.post1

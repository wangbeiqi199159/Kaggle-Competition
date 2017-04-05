Predictive Analysis of Survival Rate on Titanic
===============================================

This is a predictive machine learning project using ```R``` based on Kaggle competition: [Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic). 

To see original Kaggle post, please click [here](https://www.kaggle.com/beiqiwang/titanic/predictive-analysis-of-survival-rate-on-titanic/).
----------
**Content**

1. Introduction

      1.1 Objective

      1.2 Data Understanding

2. Data Preparation and Exploratory Analysis

      2.1 Data Cleaning

      2.2 Exploratory Analysis and Data Processing

3. Modeling

      3.1 Feature Engineering

      3.2 Model Training

      3.3 Model  Evaluation

4. Prediction

----------

## 1. Introduction

### 1.1 Objective

The sinking of the RMS Titanic is one of the most infamous shipwrecks in history.  On April 15, 1912, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. This sensational tragedy shocked the international community and led to better safety regulations for ships.

One of the reasons that the shipwreck led to such loss of life was that there were not enough lifeboats for the passengers and crew. Although there was some element of luck involved in surviving the sinking, some groups of people were more likely to survive than others, such as women, children, and the upper-class.

In this challenge, we are going to complete the analysis of what sorts of people were likely to survive.

### 1.2 Data Understanding

The data has been split into two groups:

* training set (train.csv)
* test set (test.csv)

The training set is used to build machine learning models. For the training set, we provide the outcome (also known as the “ground truth”) for each passenger. Your model will be based on “features” like passengers’ gender and class. You can also use feature engineering to create new features.

The test set should be used to see how well your model performs on unseen data. For the test set, we do not provide the ground truth for each passenger. It is your job to predict these outcomes. For each passenger in the test set, use the model you trained to predict whether or not they survived the sinking of the Titanic.

**Data Dictionary**

| Variable  |  Definition | Key  |   
|-----------|-------------|---------|
| survival  |  Survival   |  0 = No, 1 = Yes |  
|  pclass	 |  Ticket class |  1 = 1st, 2 = 2nd, 3 = 3rd |  
|  sex |  Sex |   |   
|  Age |   Age in years |   |  
|  sibsp |  # of siblings / spouses aboard the Titanic |   |   
| parch  | # of parents / children aboard the Titanic  |   |   
|  ticket | Ticket number  |   |  
|  fare | Passenger fare  |   |   
| cabin  |  Cabin number  |   |   
| embarked  | Port of Embarkation  |C = Cherbourg, Q = Queenstown, S = Southampton   |   

**Variable Notes**

pclass: A proxy for socio-economic status (SES)
1st = Upper
2nd = Middle
3rd = Lower

age: Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5

sibsp: The dataset defines family relations in this way...
Sibling = brother, sister, stepbrother, stepsister
Spouse = husband, wife (mistresses and fiancés were ignored)

parch: The dataset defines family relations in this way...
Parent = mother, father
Child = daughter, son, stepdaughter, stepson
Some children travelled only with a nanny, therefore parch=0 for them.




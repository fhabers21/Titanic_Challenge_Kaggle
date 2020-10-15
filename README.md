# Titanic: Machine Learning from Disaster
### A ML challange from [Kaggle.com](https://www.kaggle.com/c/titanic)

Goal: Use the given data to predict if a passenger would survive or not

### Score on Kaggle: 0.77751 
### Place: 5912 out of 18042 
### Best performing algorithm: RandomForestClassifier

**Feature Engineering:**

1.  Combined 'SibSp' and 'Parch' to one feature ('isAlone' = 0=yes, 1=no)
2.  Turned 'Age' into 5 groups (0-4, representing Kid-Pensioner)
3.  Turned 'Fare' into 5 groups (0-4, representing cheap-expensive)
4.  Filled in missing values for 'Age' (mean age)
5.  Filled in missing values for 'Embarked' (common value)
6.  Converting Sex (Female/Male) into numeric values 0=male, 1=female
7.  Converting Embarked (C = Cherbourg, Q = Queenstown, S = Southampton) into numeric values 0, 1 and 2
8.  Dropped Columns: Name, Ticket, Cabin (and SibSp and Parch as described in 1.)
9.  Features for training the algorithms: Pclass, Sex, Age, Fare, Embarked, isAlone

**Tested Algorithms with score on training data:**
1.  RandomForestClassifier (Score: 84.51)
2.  DecisionTreeClassifier (Score: 84.51)
3.  SupportVectorMachine (Score: 81.48)
4.  LogisticRegression (Score: 79.12)
5.  GaussianNB (Score: 77.55)
6.  SGDClassifier (Score: 74.3)

**Submitted on Kaggle (score on test data):**
1. RandomForestClassifier (0.77751)
2. DecisionTreeClassifier (0.77272)

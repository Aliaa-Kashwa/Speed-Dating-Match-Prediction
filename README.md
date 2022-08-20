# Speed-Dating-Match-Prediction

In this project, we are going to predict the outcome of a specific speed dating session based on the profile of two people, so we can implement a recommendation system to better match people in speed dating events. 
We did have another online dating dataset (Tinder-like) but that one is super dirty which requires extensive cleaning, so we do this one instead. 

This is a binary classification task. Given a data sample (information about the dating session), we are going to predict the probability (0-1, float) that the dating session will lead to a successful match.

The dataset is clean, but has a lot of missing values. The strategy for missing value replacement has to be tuned. Also, as you can guess, this dataset is highly unbalanced (mostly unmatched). 
The idea of this project is to treat the complete workflow from data preprocessing to model training as a single pipeline, and search for the hyperparameters for this pipeline. 

The notebook consists of:
1) General Questions & their answers to enhance understanding the problem domain.
2) Problem Questions & their answers to enhance understanding the problem solutions.
3) Import important libraries.
4) Import data.
    - You will find the data link in ("Link of competition on Kaggle") file attached above.
5) Data Exploration.
6) Data Visualization.
7) Data Splitting.

8) Data Preprocessing.
    - Handle Imbalanced Dataset
    - Drop unimportant columns
    - Working on Catigorical data
    
9) Choosing XGBClassifier as the model
    - Trial 1 ---> (XGBClassifier & Grid Search)
    - Trial 2 ---> (XGBClassifier & Random Search)
    - Trial 3 ---> (XGBClassifier & Bayesian Search)
    
10) Choosing LogisticRegression as the model
    - Trial 4 ---> (LogisticRegression & Grid Search)
    - Trial 5 ---> (LogisticRegression & Random Search)
    - Trial 6 ---> (LogisticRegression & Bayesian Search)

11) Test the best model on the unseen data file (test data).
12) Construct submission file.

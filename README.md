# machine-learning-challenge
Machine learning models capable of classifying candidate exoplanets from the raw dataset.

Author: Maria Barrera
Date: 05/16/2021

## Dataset:  exoplanet_data.csv

## Models used:

# 1) Logistic Regression
     Training Data Score: 0.8504672897196262
     Testing Data Score: 0.8432494279176201
     Hyperparameter tuning / Grid best score: 0.8758293976815432

The Logistic Regression initial training data score was 0.850 and the test data score was 0.843 which were similar & comparable. However, the testing generated several false positives.  The hypertuning did improve the score to 0.876.  May need to train and update X values for higher scores.

# 2) Random Forest
     Training Data Score: 1.0
     Hyperparameter tuning: 0.8920429489371919

Random Forest produces a 100% accuracy due to its algorithm.  Based on the model, may need to retest using the 4 features by their importance: koi_fpflag_ec, koi_fpflag_co, koi_fpflag_nt, and koi_fpflag_ss.

# 3) KNN
     Initial k=9 Test Acc: 1.000
     Hyperparameter tuning: 0.9640316205533598
     ** KNN point is at 9 where it stabilizes. 

The KNN point is 9 where it provides the best accuracy where the classifer starts to stabilize.  The assumption is that the data was scaled.  The data became stable after the maximum KNN range was reached.  Of all the models, KNN resulted with the highest hyperparameter tuning score of 0.96. 

Overall, after the hypertuning, all 3 models had really good scores of 0.87 or better.
Ranking of models:
     1) KNN
     2) Random Forest
     3) Logistic Regression
     

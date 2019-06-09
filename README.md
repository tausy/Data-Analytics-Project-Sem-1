# Comparison of Classification Models

## Dataset

Dataset contains 296 instances and 17 features. The dataset is suitable for classification task, where “response” represents the class while the rest of the attributes(X1..X7 and Y1..Y7) are the predictors.

## Solution approach outline

We have performed the classification task to predict the value of response attribute using the given predictor variables. We have used python 3.7 and pandas, numpy, matplotlib, sklearn and seaborn libraries to achieve the desired outcomes. We have applied Decision tree using entropy and gini index as impurity measure. We have also applied Logistic Regression with L1 penalty and Random Forest. Among all these classifiers, random forest outperformed when n_estimators=100 and max_depth=4 is used.

## Dependencies
- Python3.6+
- Pandas
- Numpy
- Sk-learn
- Matplotlib

## Steps performed in the IPython Notebook
- Dataset is loaded and printed, the NaNs are imputed with zeros.

- Dataset is described and scatter matrix plot is visualized.

- Predictors and target variable is separated and dataset is divided between train and test samples.

- Decision tree classifiers with entropy and gini are built using train split and predictions are performed using test split.

- Similarly, Logistic regression with L1 penalty and random forest classifiers are built using train split and predictions are performed using test sample.


## Results

Below results shows a comparison of all the classifiers built and their performance in terms of accuracy, precision and recall. Random Forest classifier outperformed with a better accuracy.

| Classifier | Accuracy | Precision | Recall | f1-score | support |
| ---------- | -------- | --------- | ------ | -------- | ------- |
| Decision Tree with Entropy | 68.54 | 0.70 | 0.69 | 0.68 | 89 |
| Decision Tree with Gini | 73.03 | 0.73 | 0.73 | 0.73 | 89 |
| Logistic Regression | 75.28 | 0.76 | 0.75 | 0.75 | 89 |
| Random Forest | 79.77 | 0.80 | 0.80 | 0.80 | 89 |


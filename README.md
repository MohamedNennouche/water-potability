# Drinking Water Classification Project
## Goal of the project
The goal of this project is to implement a binary classification model, we have in our dataset, found on Kaggle at [this link](https://www.kaggle.com/adityakadiwal/water-potability) and thus at the level of the dataset we have 10 variables which are : 
- ph
- Hardness
- Solids
- Chloramines
- Sulfate
- Conductivity
- Organic_carbon
- Trihalomethanes
- Turbidity
## Structure of the project 
- water-notebook.ipynb : The Jupyter notebook where the project is made
- water_potability : csv file downloaded from Kaggle containing our problem
## Some remarks 
- The project is a binary classification problem
- There are a number of rows that do not contain all the values, the method chosen in this project to remedy this is to delete them as noticing that their deletion impacts very little the global distribution of variables
## Software requirements 
This project is made with Python so for the use or the copy of this project you will need : 
- Python 3.8 and up 

The following Python packages: 
- Numpy
- Matplotlib (and especially the pyplot module)
- Pandas
- Scikit-learn
- Seaborn
- lightgbm
- xgboost
## Performance achieved with selected models
|   Algorithms    |   Accuracy (%)    |   F1-score (%)    |   ROC-Auc score (%)    |
|---                                |:-:    |:-:    |:-:    |
| KNN                               | 63.41 | 56.06 | 58.02 |
| MLP                               | 63.41 | 62.18 | 62.16 |
| SVM                               | 67.88 | 62.65 | 63.26 |
| NuSVM                             | 67.55 | 65.03 | 64.84 |
| Random Forrest                    | 68.21 | 64.38 | 64.44 |
| Gaussian Naive Bayes              | 30.60 | 52.76 | 55.15 |
| Gradient Boosting                 | 65.23 | 60.35 | 60.95 |
| LGBM                              | 68.54 | 63.10 | 63.77 |
| Catboost                          | 67.38 | 64.01 | 63.98 |
| XGBoost                           | 65.73 | 63.38 | 63.23 |
| Gaussian Processes                | 67.72 | 63.42 | 63.66 |
| Extremely randomized tree         | 69.37 | 64.54 | 64.89 |
| Histogram-Based Gradient Boosting | 63.41 | 60.22 | 60.29 |
## Performances achieved with a Learning set 
The following results can be found:

|   Voting method chosen    |   Accuracy (%)    |   F1-score (%)    |   ROC-Auc score (%)    |
|---                                |:-:    |:-:    |:-:    |
|   Hard voting    |   69.37    |   64.43    |   64.83    |
|   Soft voting    |   68.71    |   64.72    |   64.81    |
## Performance achieved with resampling

## To-do
- [x] Add a resampling and see its effect
- [ ] Add feature selection methods 
- [ ] Apply principal component analysis to improve performance
- [ ] Features engineering using polynomial inputs
- [ ] Complete the README
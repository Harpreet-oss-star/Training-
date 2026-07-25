*WEEK 4
Day 1
Date: 20 jyly 2026*

Linear Regression, Ridge Regression and Lasso Regression :
These are supervised learning algorithms mainly used for regression problems, where the target is a continuous numerical value.

1. Linear Regression :
Linear Regression predicts a numerical value by finding the relationship between input features and the target.

Example applications:

Predicting house prices
Predicting temperature
Predicting student marks

2. Ridge Regression :
Ridge Regression is Linear Regression with L2 Regularization.
It adds a penalty for large coefficients to reduce overfitting.

Reduces overfitting
Works well when features are highly correlated
Reduces coefficient values
Usually keeps all features

3. Lasso Regression :
Lasso Regression is Linear Regression with L1 Regularization.
It can reduce some feature coefficients to exactly zero.
The feature with coefficient 0 is effectively removed.

Therefore, Lasso performs:
Regression + Feature Selection

*Day 2
Date: 21 jyly 2026*

Feature Selection Methods

Feature selection means selecting the most useful features from a dataset and removing irrelevant or redundant features. This can improve model performance, reduce training time, and reduce overfitting.

Types of feature selection:
Filter Method
Wrapper Method
Embedded Method

FILTER METHOD :
Filter methods select features using statistical techniques without training a machine learning model.

1. Variance Thresholding :
This method removes features that have very little variation.
If a feature has almost the same value for every row, it usually provides little useful information.
Best for: Removing constant or nearly constant features.

2. Chi-Squared Test :
The Chi-Squared Test is used to select important categorical features for a classification problem.
It checks whether a categorical feature has a significant relationship with the target.

3. Mutual Information :
Mutual Information measures how much information a feature provides about the target.
If a feature contains useful information for predicting the target, its mutual information score will generally be higher.
Best for: Classification problems and detecting nonlinear relationships.

4. F-Test (ANOVA) :
The ANOVA F-Test checks whether the mean values of a numerical feature are significantly different across different target classes.
Best for: Numerical features and categorical classification targets.

*Day 3
Date: 22 jyly 2026*

WRAPPER METHOD :
Wrapper methods select features by training and testing a machine learning model with different combinations of features.

1. Forward Selection

Forward Selection starts with zero features and adds features one by one.
At every step, the feature that improves the model the most is added.
Advantage: Useful when you have many features and want to build the model gradually.

2. Backward Elimination

Backward Elimination starts with all features and removes the least useful feature one by one.
The process continues until the best feature combination is found.

3. RFECV

RFECV = Recursive Feature Elimination with Cross-Validation
It repeatedly removes the least important features and uses cross-validation to determine the best number of features.

*Day 4
Date: 23 jyly 2026*

Hyperparameter Tuning :

Hyperparameter tuning is the process of finding the best values for a machine learning model's hyperparameters to improve its performance.

A hyperparameter is a setting that is decided before model training.

# Random Forest
Hyperparameter	Meaning
n_estimators -	Number of trees
max_depth	- Maximum depth of each tree
min_samples_split -	Minimum samples required to split a node

# KNN
Hyperparameter	Meaning
n_neighbors	- Number of nearest neighbors
weights	- How neighbors contribute
metric -	Distance calculation method

# SVM
Hyperparameter	Meaning
C	- Controls penalty for errors
kernel -	Type of decision boundary
gamma	- Influence of individual data points


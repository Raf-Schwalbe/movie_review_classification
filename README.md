
# Movie review classification

Purpose of the analysis is to build a classification model 
that is able to classify whether review was positive or negative

Firstly classical classification methods are used (main). 

Secondly neural network is checked (main_nn)




## Table of contents

### EDA and classic classification methods (main)

- Introduction - what do we want to achieve?
- Exploratory Data Analysis
  - Variation
    - Outliers
    - Only 0 observations
  - Covariation
- Modelling
  - Models - filter model selection - SelectKBest
  - Models - RFCV model selection
  - Model results
  - Hyperparameters tuning for top model.
- Best model Interpretation
  - Performance
  - Metrics
  - Validation curves
  - Independent variables p-value check
  - Feature importance
- Summary

### Neural network (main_nn)

- Introduction
- Modelling 
  - Hyperparameters tunning
- Interpretation
- Summary
- Scikit learn w Keras


## Interesting features

- cross validation where estimator (for RFECV) and classification algorithm) are assesed.


## Results

- The best model is Logisitc regression with features selected with Logistic regression. Its mean accuracy was 82,63%

- In general:

  - tree based models performed visibly worse
  - the estimator used in RFCV did not really matter  unless it was decision tree which worsened model performance
  - models with feature selected with filter method performs worse than with RFCV unless they are tree based.

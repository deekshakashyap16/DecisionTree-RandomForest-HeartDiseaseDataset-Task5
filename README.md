# Task 5: Decision Trees and Random Forests (Heart Disease Dataset)

This repository contains my solution for Task 5, focusing on implementing and evaluating Decision Tree and Random Forest classifiers using the Heart Disease dataset.

### What did I do?

he goal was to learn about tree-based models, understand concepts like overfitting and feature importance, and compare the performance of a single Decision Tree against a Random Forest ensemble using Scikit-learn.

### Decision Tree

DecisionTreeClassifier was trained without depth limits. It achieved 1.0 training accuracy and 0.985 test accuracy, showing slight overfitting. The tree was visualized using plot_tree for better understanding.

### Pruning and Depth Control

Pruning was applied using max_depth=4, min_samples_split=10, and min_samples_leaf=5. This reduced overfitting but also lowered accuracy (0.879 train, 0.795 test). Varying the depth showed that performance was best around depth = 8.

### Random Forest

RandomForestClassifier (n_estimators=200, max_depth=8) performed best overall compared to the earlier n_estimators=100. It achieved 0.996 training and 0.980 testing accuracy, offering a good balance between bias and variance.

### Feature Importance

Feature importances were extracted from the Random Forest model to identify the most influential variables.

### Cross-Validation

5-fold cross-validation gave a mean accuracy of 0.974, confirming stable and reliable model performance.

### Tools and Libraries
Scikit-learn, Matplotlib, Pandas, Graphwiz
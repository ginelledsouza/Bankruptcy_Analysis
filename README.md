# Bankruptcy Analysis

This repository aims at analyzing the possibility of whether an organization would face bankruptcy. 
The main focus of this repository is to demonstrate concepts listed as follows:

- **Dealing with imbalanced datasets the right way** <br>
An imbalanced dataset is a situation when there is an unequal distribution of classes in the dataset. 
We can solve this by either upsampling - introducing minority class at power with majority class or downsampling - reducing majority 
class to match the size of minority class. The dataset we are analyzing is highly imbalanced. Thus before training the model, we need to deal with this data. 
Let us lay down some steps we must follow when we come across an imbalanced dataset.<br>
-- Split the dataset into training and testing sets (80% - 20%). We preserve the 20% testing set for the final evaluation.<br>
-- Through "Stratified K Fold Cross-Validation" we will now distribute the 80% training set into further training and testing splits.<br>
-- Since we are dealing with over 50 features, we use "Randomized Search Cross-Validation" as this technique proves to perform better with many features.
<br>

- **Finding the best attributes to work with through feature selection** <br>
We are now dealing with over 50 attributes in this dataset, let us just play around and demonstrate how we can 
programmatically pick the best features, and analyze how it affects our model.


# Analysis Findings / Outcomes
|  Algorithm | Model Score  | F1 score  |
|---|---|---|---|---|
|  Random Forest Classifier | 98.9% |  0.86 |
|  K Nearest Neighbour | 98.02%  | 0.78 |
|  Support Vector Classifier | 95.82%  | 0.62 |
|  Logistic Regression | 89.22%  | 0.36 |
|  DecisionTree Classifier | 85.26%  | 0.32 |


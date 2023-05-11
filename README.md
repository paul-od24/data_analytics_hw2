# data_analytics_hw2
Homework 2 as part of data analytics module.
The goal in this homework is to work with the data to build and evaluate prediction models that capture the relationship between the descriptive features and the target feature **death_yn**.
For this homework we will use the same dataset allocated to us in Homework1.

# Task 1: Data Understanding and Preparation
In this task, we explore the relationships between feature pairs and select/transform promising features based on a given training set. The following steps are performed:

1.1 Splitting the Dataset: The dataset is split into two datasets: a 70% training set and a 30% test set. The test set is kept aside for evaluation purposes.
1.2 Feature Analysis: On the training set:
Correlation Analysis: Correlations between all continuous features are plotted to observe any existing relationships.
Continuous Feature Interaction: For each continuous feature, its interaction with the target feature is plotted. Promising continuous features are selected based on their ability to predict the target feature.
Categorical Feature Interaction: Pairwise interaction between each categorical feature and the target feature is plotted. Promising categorical features are chosen based on their predictive power.

# Task 2: Predictive Modeling with Linear Regression
This task focuses on building a linear regression model for predicting the target feature. The following steps are performed:

2.1 Linear Regression Training: Using the training set, a linear regression model is trained to predict the target feature. Only the descriptive features selected in Task 1 are used.
2.2 Coefficient Analysis: The learned coefficients of the linear regression model are printed and discussed to understand their role in the model.
2.3 Prediction and Evaluation: The predicted target feature values for the first 10 training examples are printed. These predicted values are thresholded at 0.5 to obtain the predicted classes. Classification evaluation measures such as accuracy, confusion matrix, precision, recall, and F1 score are computed on the full training set to assess the model's performance.
2.4 Model Evaluation: The trained linear regression model is evaluated using classification evaluation measures on the hold-out (30%) test set. The evaluation results are compared with those obtained on the training dataset. Additionally, the model's performance is compared to a cross-validated model trained and evaluated using k-fold cross-validation or repeated train/test splits.

# Task 3: Predictive Modeling with Logistic Regression
This task involves training a logistic regression model to predict the target feature. The following steps are performed:

3.1 Logistic Regression Training: A logistic regression model is trained on the training set using the selected descriptive features.
3.2 Coefficient Analysis: The learned coefficients of the logistic regression model are printed and analyzed to understand their role in the model.
3.3 Prediction and Evaluation: The predicted target feature values and predicted classes are printed for the first 10 training examples. Classification evaluation measures such as accuracy, confusion matrix, precision, recall, and F1 score are computed on the full training set to evaluate the model's performance.
3.4 Model Evaluation: The logistic regression model is evaluated using classification evaluation measures on the hold-out test set. The evaluation results are compared with those obtained on the training dataset and the cross-validated model.

# Task 4: Predictive Modeling: Random Forest.  
This task focuses on building a random forest model for predicting the target feature. The following steps are performed:

4.1 Random Forest Training: On the training set, a random forest model is trained using the selected descriptive features from Task 1.
4.2 Model Interpretation: An attempt is made to interpret the random forest model and gain insights into its working and behavior. Knowledge gained from this analysis is discussed.
4.3 Prediction and Evaluation: The predicted target feature values and predicted classes are printed for the first 10 training examples. Classification evaluation measures such as accuracy, confusion matrix, precision, recall, and F1 score are computed on the full training set to assess the model's performance.
4.4 Model Evaluation: The model is evaluated using classification evaluation measures on the hold-out test set. The evaluation results are compared with the results obtained on the training dataset. Additionally, the performance of the model is compared with a cross-validated model that is trained and evaluated using k-fold cross-validation or repeated train/test splits. The cross-validation metrics are compared to those obtained from the single train/test split and the random forest out-of-sample error. The findings of these comparisons are discussed.

# Task 5: Improving Predictive Models
This task involves exploring ideas to improve the predictive models trained so far. The following steps are performed:

5.1 Model Performance Evaluation: The performance of the trained models is assessed to determine which model performs better at predicting the target feature. A comparison is made with a simple model that always predicts the majority class. Justifications are provided for the chosen model based on its accuracy.
5.2 Summary and New Ideas: A summary is provided, outlining the understanding of the problem and the results obtained from the predictive modeling tasks. Ideas for further improvement of the best model are presented, including feature selection, feature re-scaling, creation of new features, model combination, or leveraging domain knowledge. Code is implemented to train and evaluate the proposed models, and the findings are summarized.

# Authors:
Paul O'Donovan - paul-od24 <br>
David Mallon - D-Mallon

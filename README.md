# Titanic Passenger Survival Prediction
## Project Overview:
I worked on the Titanic dataset available on Kaggle, aiming to predict the survival of passengers based on various features. The project involved several steps including data preprocessing, feature engineering, model training, hyperparameter tuning, and evaluation of various machine learning algorithms.

### 1. Data Preprocessing and Feature Engineering:
Data Cleaning:
Addressed missing values in the dataset. For instance, the missing values in the Age feature were imputed using the median age grouped by Pclass and Sex. The Embarked feature, which also had missing values, was imputed with the mode.
Feature Engineering:
1. Family Size: Created a new feature by combining the number of siblings/spouses aboard (SibSp) and the number of parents/children aboard (Parch), and adding one to include the passenger themselves.
2. Family Size Grouped: Categorized family sizes into groups such as solo (traveling alone), small (traveling with a few family members), and large (traveling with many family members).
3. Ticket Location: Extracted information from the ticket numbers, assuming certain patterns might indicate different sections or classes within the ship.

### 2. Feature Selection:
Dropped unnecessary or redundant features that were not contributing significantly to the model's predictive power. This included features like PassengerId, Ticket, and Cabin after extracting useful information.

### 3. Model Training:
Algorithms Applied:
Logistic Regression: A simple linear model suitable for binary classification.
Support Vector Machine (SVM): Effective for high-dimensional spaces.
Decision Tree: A non-linear model that splits the data based on feature values.
Random Forest: An ensemble method using multiple decision trees to improve performance.
K-Nearest Neighbors (KNN): A non-parametric method that classifies based on the majority class among the nearest neighbors.
Naive Bayes: A probabilistic classifier based on Bayes' theorem with strong independence assumptions between features.

### 4. Hyperparameter Tuning:
Optimized the models using techniques like GridSearchCV and RandomizedSearchCV to find the best parameters for ensemble algorithms such as AdaBoost and Gradient Boosting.

### 5. Model Evaluation:
Evaluated each model using several metrics:
Accuracy: The ratio of correctly predicted instances to the total instances.
Precision: The ratio of true positive predictions to the total predicted positives.
Recall: The ratio of true positive predictions to the total actual positives.
F1 Score: The harmonic mean of precision and recall, providing a balance between the two.

### 6. Model Selection and Final Training:
Based on the evaluation metrics, selected Gradient Boosting as the final model for its superior performance.

### 7. Final Submission:
Applied the Gradient Boosting model to the test dataset.
Submitted the predictions to Kaggle, achieving a score of 0.76794 out of 1.0, placing me in the top 17%.


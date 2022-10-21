# Diabetes Prediction

This is the final project of MSSP 608 Machine Learning.


# Data Source

## Links
* Link of data source: https://www.kaggle.com/datasets/mathchi/diabetes-data-set
* Link of google colab: https://drive.google.com/file/d/1bMWDjdJgT47th7IsPfgkaRYc_3lZiX5H/view?usp=sharing

## Data Description
We will use a dataset in Kaggle which contains features used to predict diabetes.

Our original dataset contains 8 features and 1 label, with a total of 768 patient-level observations. Our label is a binary variable where 0 equals no diabetes and 1 equals diabetes. The data was collected by the National Institute of Diabetes and Digestive and Kidney Diseases.

During data preprocessing, we removed 44 patients which we identified as outliers, leaving a remaining 724 patients included in our model's train & test datasets.
.

# Model Building
We implement supervised models and unsupervised models to predict the occurence of diabetes.

a) Supervised Models: Naïve Bayes, Logistic Regression, SVMs, Decision Trees, Random Forests, and Adaboost.
b) Unsupervised Models: PCA, K-Means

# Conclusion
## Best performing model
Overall, the logistic regression hold-one-out model performed the best, with an accuracy score of 0.79 and a kappa score of 0.51

## Feature importance
"Age" and "Glucose" are proven to be the most important ones in predicting diabetes.

## Challenges
### Hyperparameter tuning 
We might need to spend more time experimenting with the parameters that can optimize the performance of our chosen model
### Sample size
The number of obeservations is quite limited. In particular, this dataset contains female patients only. As a result, our models might not be accurate enough, especially if we want to generalize to the whole population.
### Specification.
Since in clinical practice, "Glucose" is already used as a index to diagnose diabetes. The effect of our research in identifying potential features that can predict diabetes greatly diminishes.


## Potential Next Steps
* We could continue to tune our models, to achieve better performances (potentially)
* We could take a step further, to study which factors will have an impact on Glucose, BMI, etc. 

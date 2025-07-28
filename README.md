# HR-Analytics-Employee-Prediction
This project uses machine learning to predict employee promotions based on various performance and demographic factors. It aims to help HR departments make data-driven decisions about which employees are most likely to be ready for a promotion.

# Project Overview
The goal of this project is to build a predictive model that can identify employees who are strong candidates for promotion.[1][2] By analyzing historical data on employee attributes and promotion outcomes, we can uncover patterns and create a model that assists in making fair and efficient promotion decisions.[1][3] This data-driven approach helps to streamline the promotion process and reduce delays in transitioning employees to new roles.

# Dataset
The dataset used in this project contains information about employees, including:
* department: The department the employee works in.
* region: The geographical region of employment.
* education: The employee's level of education.
* gender: The gender of the employee.
* recruitment_channel: The channel through which the employee was recruited.
* no_of_trainings: The number of training courses the employee has completed.
* age: The age of the employee.
* previous_year_rating: The employee's performance rating from the previous year.
* length_of_service: The number of years the employee has been with the company.
* KPIs_met >80%: Whether the employee has met more than 80% of their Key Performance Indicators (KPIs).
* awards_won?: Whether the employee has won any awards.
* avg_training_score: The employee's average score in training evaluations.
* is_promoted: The target variable, indicating whether the employee was promoted.
# Methodology
The project follows these key steps:
1. Data Preprocessing and Exploratory Data Analysis (EDA): This involves cleaning the data, handling missing values, and exploring the relationships between different variables. For example, missing values in the 'education' and 'previous_year_rating' columns were filled in. Categorical features were also converted into numerical format using LabelEncoder.
2. Feature Engineering: The 'employee_id' column was dropped as it is not relevant for prediction.
3. Model Building: A Decision Tree Classifier was chosen to predict employee promotions. This model is well-suited for classification tasks and provides interpretable results.
4. Hyperparameter Tuning: To optimize the model's performance, GridSearchCV was used. This technique systematically searches for the best combination of hyperparameters to improve the model's predictive accuracy. The hyperparameters tuned for the Decision Tree include criterion, max_depth, min_samples_split, and min_samples_leaf.
5. Model Evaluation: The model was evaluated using various metrics, including accuracy, precision, recall, F1-score, and the ROC AUC curve. These metrics provide a comprehensive assessment of the model's performance.
# Results
After training and tuning, the Decision Tree model achieved the following performance on the test set:
* Accuracy: 93.36%
* Precision: 80.61%
* Recall: 26.1%
* F1-score: 39.43%
* AUC: 0.87

The high accuracy indicates that the model is effective at predicting whether an employee will be promoted. However, the lower recall score suggests that the model may miss some employees who were actually promoted.
# How to Use This Project
To use this project, you will need to have Python and the following libraries installed:
* pandas
* numpy
* seaborn
* matplotlib
* scikit-learn

You can then run the Jupyter notebook to see the code and results.
# Conclusion
This project demonstrates the potential of using machine learning for HR analytics, specifically for predicting employee promotions. By leveraging data, organizations can make more informed and equitable decisions that benefit both the employees and the company. Future work could involve exploring other machine learning models or gathering more data to further improve the model's performance.

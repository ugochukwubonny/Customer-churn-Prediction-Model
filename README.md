# Customer-churn-Prediction-Model
Overview
This project involves building a churn prediction model using logistic regression to classify customers as likely to churn or not. The model was developed using a dataset with various customer attributes and was evaluated on its ability to accurately predict customer churn.

Dataset
The dataset used for this model includes the following features (columns):

Age: The age of the customer.
Gender: The gender of the customer.
Tenure: The number of months the customer has been with the company.
Usage Frequency: How often the customer uses the service.
Support Calls: The number of support calls made by the customer.
Payment Delay: The frequency of payment delays by the customer.
Subscription Type: The type of subscription the customer has.
Contract Length: The length of the customer's contract.
Total Spend: The total amount spent by the customer.
Last Interaction: The time since the customer's last interaction with the service.
Packages Used
The following Python packages were used to build and evaluate the model:

pandas: For data manipulation and analysis.
matplotlib.pyplot: For plotting and visualizing data.
plotly.express: For interactive plots and visualizations.
numpy: For numerical computations.
warnings: To handle and ignore warnings.
glob: To find files matching a specified pattern.
sklearn.linear_model.LogisticRegression: For building the logistic regression model.
sklearn.impute.SimpleImputer: For handling missing data.
category_encoders.OneHotEncoder: For encoding categorical variables.
sklearn.model_selection.train_test_split: For splitting the data into training and test sets.
sklearn.metrics.accuracy_score: For evaluating model accuracy.
sklearn.pipeline.make_pipeline: For creating a pipeline of preprocessing and modeling steps.
Exploratory Data Analysis (EDA)
Before building the model, an exploratory data analysis (EDA) was conducted to understand the dataset and the relationships between features. This included:

Checking for missing values and handling them appropriately.
Visualizing distributions of numerical features.
Exploring relationships between features and the target variable (churn).
Encoding categorical variables for use in the model.
Model Building
The churn prediction model was built using logistic regression, which is suitable for binary classification tasks. The model pipeline includes:

SimpleImputer: To fill missing values with the mean of the column.
OneHotEncoder: To encode categorical variables into a format suitable for logistic regression.
LogisticRegression: The classifier used to predict churn.

Model Training and Evaluation
The dataset was split into training and test sets using an 80-20 split.
The model was trained on the training set and evaluated on the test set.
The test accuracy of the model was found to be 0.83, indicating that the model correctly predicts customer churn 83% of the time.
The baseline accuracy, assuming the most frequent class, was 0.55%. Thus, the model significantly outperforms the baseline.

Conclusion
The churn prediction model achieved a test accuracy of 83%, demonstrating its effectiveness in predicting customer churn. This model can be a valuable tool for the company to identify customers at risk of churning and take proactive measures to retain them.

Future Work
Feature Engineering: Further feature engineering could be performed to enhance model performance.
Model Tuning: Hyperparameter tuning and trying other classification algorithms could improve accuracy.
Deployment: The model can be deployed in a production environment for real-time churn prediction.

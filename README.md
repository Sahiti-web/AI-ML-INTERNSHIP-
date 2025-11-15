# AI-ML-INTERNSHIP-
Task 1: Data Cleaning and Preprocessing (Titanic Dataset).
🎯 Objective
To clean and prepare the raw Titanic dataset for machine learning model training.
🛠 Script: data_preprocessing.py
This script executes the necessary data cleaning and feature engineering steps:
1. Handling Missing Data (Imputation)
Cabin: Dropped due to being over 77% missing.
Age: Imputed with the median value.
Embarked: Imputed with the mode (most frequent port).
2. Feature Selection & Encoding
Dropped: Irrelevant columns PassengerId, Name, and Ticket.
Sex: Encoded using Label Encoding (Male=1, Female=0).
Embarked: Encoded using One-Hot Encoding (pd.get_dummies) to maintain categorical independence.
3. Outlier and Scale Management
Outliers (Fare): Detected using the IQR method (Box Plot visualization). Extreme values were handled by Capping (Winsorization) to mitigate skewing effects.
Scaling: Both Age and Fare were scaled using Standardization (Z-score), setting the mean to 0 and the standard deviation to 1. This ensures all numerical features are on the same scale for the model.
🚀 How to Run It
Place data_preprocessing.py and Titanic-Dataset.csv in the same directory.
Run the script in your terminal:
python data_preprocessing.py


(P.S. Detailed answers to the interview questions are in interview_qa.md)

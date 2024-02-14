# Customer Churn Prediction Project

This project involves building a machine learning model to predict customer churn based on various features from a telecommunications company's dataset. The goal is to identify customers who are likely to churn so that proactive measures can be taken to retain them.

## Dataset

The dataset, `Customer Churn Data.csv`, includes multiple features such as customer demographics, account information, and charges. The target variable is `Churn`, which indicates whether a customer has left the company (Yes or No).

## Methodology

The project follows these steps:

1. **Data Loading**: Load the dataset using pandas and display the first few rows to understand its structure.

2. **Exploratory Data Analysis (EDA)**:
   - Visualize the distribution of key categorical variables.
   - Analyze the relationship between monthly charges and churn using a boxplot.

3. **Data Preprocessing**:
   - Handle missing values in `TotalCharges` by converting them to numeric and dropping any errors.
   - Encode categorical features using Label Encoding to transform them into a format suitable for machine learning models.
   - Merge categorical and numerical features into a final dataframe, dropping unnecessary columns like `customerID`.
   - Address class imbalance using SMOTE (Synthetic Minority Over-sampling Technique).

4. **Model Building**:
   - Split the data into training and testing sets.
   - Train a RandomForestClassifier on the oversampled training data.
   - Evaluate the model on the test set using accuracy, confusion matrix, and classification report.

## Key Python Libraries Used

- `pandas` for data manipulation and analysis.
- `numpy` for numerical operations.
- `matplotlib.pyplot` and `seaborn` for data visualization.
- `sklearn` for model building, data preprocessing, and performance evaluation.
- `imblearn.over_sampling` for handling class imbalance with SMOTE.

## Results

The performance of the model is evaluated using the accuracy score, confusion matrix, and classification report. These metrics provide insights into the model's ability to predict churn accurately.

## Conclusion

This project demonstrates the process of building a predictive model for customer churn. It includes data preprocessing, exploratory data analysis, model training, and evaluation. The RandomForestClassifier model, along with SMOTE for handling imbalanced data, offers a solid approach to predicting customer churn.

## How to Run

Ensure you have Python installed and the required libraries mentioned above. Place the dataset in the appropriate directory and execute the script. Adjust the file path as necessary.


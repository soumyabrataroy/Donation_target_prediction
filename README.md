# Donation_target_prediction

The goal is to build a classifier that predicts income levels based on a person's attributes, such as education, job, and ethnicity. The script performs the following steps:

1. **Data Import and Cleaning:**
    - Imports the necessary libraries for data analysis and modeling.
    - Reads the dataset from a CSV file and assigns column names.
    - Checks for missing values and removes any rows with missing data.
    - Strips white space characters from the income column.

2. **Exploratory Data Analysis:**
    - Calculates and prints the number of records, number of individuals with income greater than $50,000, and number of individuals with income at most $50,000.
    - Calculates and prints the percentage of individuals with income greater than $50,000.
    - Creates histograms for age, capital gain, and capital loss.
    - Transforms skewed data (capital gain and capital loss) using the logarithmic function.

3. **Data Preparation:**
    - Drops the 'fnlwgt' column as it is not relevant for the analysis.
    - Encodes categorical features using one-hot encoding.
    - Encodes the income column into numerical values.
    - Splits the data into training and testing sets.

4. **Model Training and Evaluation:**
    - Trains three different classifiers (Decision Tree, SVM, and AdaBoost) on the training data.
    - Evaluates each model's accuracy and F-score on the training and testing sets.
    - Compares the performance of the three models and selects the best one (AdaBoost) based on its performance on the testing data.

5. **Model Optimization:**
    - Performs grid search on the AdaBoost classifier to find the optimal hyperparameters.
    - Trains the optimized model on the training data and evaluates its performance on the testing data.

6. **Feature Importance:**
    - Extracts the feature importances from the optimized model.

The script provides a comprehensive example of how to perform data analysis and modeling to predict income levels based on a person's attributes. It demonstrates the use of various data cleaning, exploration, preparation, and modeling techniques. The script also highlights the importance of model optimization and feature importance analysis.
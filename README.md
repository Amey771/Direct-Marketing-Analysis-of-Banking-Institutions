# Data Mining Final Project Report

## Executive Summary

This project focuses on a classification task for a Portuguese banking institution's direct marketing campaign. By predicting whether a client will subscribe to a term deposit, multiple classification models were evaluated. **Logistic Regression** achieved the best performance with a 91% accuracy, indicating a strong linear boundary in the dataset.

---

## Overview

This repository contains the final project for the Data Mining course. The objective is to develop a robust predictive model to assess the success of marketing campaigns by analyzing both customer demographics and socio-economic factors. The project covers comprehensive steps from data preprocessing to model evaluation.

---

## Problem Statement

The goal of this project is to predict the success of direct marketing campaigns executed via phone calls by a Portuguese banking institution. Specifically, the task is to determine whether a client will subscribe to a term deposit ('y') based on a wide array of input features such as demographics, economic indicators, and campaign-related variables.

---

## Dataset

The primary dataset used is **"bank-additional-full.csv"**, which includes:
- **41,188 examples** with 20 input variables.
- **Input variables** include: age, job type, marital status, education, default status, housing loan, personal loan, contact details, campaign information, and various economic indicators.
- **Target variable:** `y` (indicating whether the client subscribed to a term deposit).

---

## Preprocessing

Key preprocessing steps include:
- **Column Renaming:** Standardizing column names by replacing periods with underscores.
- **Missing Value Handling:** Imputing missing values using the median for numerical features and the mode for categorical features.
- **Feature Selection:** Removing highly correlated numerical features to reduce multicollinearity.
- **Encoding:** Converting categorical variables into numerical representations using OneHotEncoder and LabelEncoder.
- **Data Splitting:** Partitioning the data into training, validation, and test sets.

---

## Data Organization

Data was organized into distinct processing pipelines:
- **Numerical Pipeline:** Handling imputation and scaling.
- **Categorical Pipeline:** Applying one-hot encoding and label encoding.
This structured approach ensured clarity during data manipulation and set a strong foundation for model training.

---

## Results

Several classifiers were implemented and compared:
- **KMeans:** 89% accuracy  
- **KNearest Neighbors:** 90% accuracy  
- **Random Forest:** 89% accuracy  
- **Decision Tree:** 83% accuracy  
- **Logistic Regression:** **91% accuracy**  
- **Naive Bayes:** 81% accuracy  
- **Support Vector Classifier:** 88% accuracy  
- **Gradient Boosting:** 88% accuracy  

The evaluation was based on confusion matrices, precision, recall, and f1-scores. Logistic Regression emerged as the top performer.

---

## Classifier Performance

The performance metrics indicate:
- **Logistic Regression** provided the best overall performance with the highest accuracy and superior f1-scores for both classes.
- Each model was analyzed using a confusion matrix to assess the balance between true positives and true negatives, with special focus on the model’s ability to predict the positive class.

---

## Conclusion

The analysis confirms that Logistic Regression is the most effective classifier for this dataset, achieving a 91% accuracy rate. The preprocessing strategies and evaluation methods played a critical role in optimizing model performance, demonstrating the importance of thorough data preparation in predictive modeling.

---

## Future Work

Potential future directions include:
- Enhancing visualization techniques for high-dimensional data.
- Implementing more sophisticated grid searches and advanced feature engineering methods.
- Addressing class imbalance using oversampling techniques.
- Utilizing high-performance computing (e.g., GPU acceleration) to speed up model training, especially for computationally intensive models like SVC.

---

## Team & Credits

**Team 4:**  
- Amey Borkar  
- Shivam Joshi  
- Lolyna de la Fuente  
- Can Demirel  
- Joseph Ng  

Special thanks to all team members for their contributions. This project was completed as part of the Data Mining course, and the comprehensive analysis has provided valuable insights into direct marketing effectiveness.

---

For more details, please refer to the full project report included in this repository.

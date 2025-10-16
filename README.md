# Rock vs. Mine Prediction using Sonar Data

This project uses machine learning to classify underwater objects as either Rocks or Mines based on sonar signal data. A Logistic Regression model is trained to perform this binary classification task.

## Project Overview

The goal of this project is to build a predictive model that can accurately distinguish between metallic (mines) and non-metallic (rocky) objects from their sonar returns. The entire machine learning pipeline, from data exploration to building a predictive system, is implemented in the `RockVsMine.ipynb` Jupyter Notebook.

## Dataset

The dataset used is the "Sonar, Mines vs. Rocks" dataset, which contains 208 instances and 60 features representing the energy in different frequency bands. The 61st column is the label, where 'M' stands for Mine and 'R' for Rock.

- **Number of Instances:** 208
- **Number of Features:** 60
- **Class Distribution:**
    - Mine (M): 111
    - Rock (R): 97

## Methodology

1.  **Data Loading & Analysis:** The dataset is loaded using Pandas for initial exploration and statistical analysis.
2.  **Data Preprocessing:** Features (X) and the target variable (Y) are separated.
3.  **Train-Test Split:** The data is split into training (90%) and testing (10%) sets using Scikit-learn's `train_test_split`. Stratification is used to ensure a balanced class distribution in both sets.
4.  **Model Training:** A Logistic Regression classifier is trained on the training data.
5.  **Model Evaluation:** The model's performance is evaluated using accuracy scores and classification reports for both training and testing sets to check for generalization.
6.  **Predictive System:** A simple system is built to take new sonar data as input and predict whether the object is a Rock or a Mine.

## Results

-   **Training Data Accuracy:** 83.4%
-   **Test Data Accuracy:** 76.2%

The classification reports provide a more detailed look at the precision, recall, and F1-score for each class.

## Technologies Used

-   Python
-   Pandas
-   NumPy
-   Scikit-learn
-   Jupyter Notebook

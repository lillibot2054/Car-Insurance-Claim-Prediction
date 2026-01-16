

#  Car Insurance Claim Prediction 

##  Project Overview

This project focuses on predicting whether an insurance policyholder will file a claim using machine learning techniques. The goal is to build, evaluate, and compare multiple classification models while handling real-world challenges such as categorical data, class imbalance, and feature preprocessing.

The project follows an **end-to-end ML pipeline**, from data preprocessing to model evaluation and final submission generation.

---

##  Dataset

The dataset consists of policyholder information provided in three files:

* `train.csv` – Training data with target variable
* `test.csv` – Test data without target
* `sample_submission.csv` – Submission format template

**Target Variable**

* `is_claim` → Binary indicator of whether a claim was made

---

##  Methodology

### 1️⃣ Data Preprocessing

* Automatic detection of numerical and categorical features
* Numerical features scaled using **StandardScaler**
* Categorical features encoded using **OneHotEncoder**
* Preprocessing handled through **Scikit-learn Pipelines** to avoid data leakage

### 2️⃣ Train–Validation Split

* 80% training / 20% validation split
* Stratified sampling to preserve class distribution

---

##   Models Implemented

### 🔹 Baseline Model 1 – Logistic Regression

* Handles class imbalance using `class_weight='balanced'`
* Evaluated using Accuracy, Precision, Recall, F1-Score, and ROC-AUC

### 🔹 Baseline Model 2 – Decision Tree

* Controlled depth to reduce overfitting
* Balanced class weights
* Evaluated using F1-Score and ROC-AUC

### 🔹 Baseline Model 3 – Random Forest (Final Model)

* Ensemble of multiple decision trees
* Improved generalization and robustness
* Feature importance analysis performed
* Used for final test predictions

---

##   Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC
* Confusion Matrix visualization

These metrics provide a comprehensive view of performance, especially for imbalanced classification problems.

---

##   Final Model

The **Random Forest classifier** demonstrated the best overall performance and was selected as the final model. It was used to generate probability predictions for the test dataset and create the final submission file.

---

##   How to Run

1. Clone the repository
2. Open the notebook in **Google Colab** or **Jupyter Notebook**
3. Import the dataset & unzip it
4. Run cells sequentially (top to bottom)
5. The final submission file will be saved as:

   ```
   Final_Submission_Updated.csv
   ```

---

##   Key Learnings

* Importance of pipelines for clean ML workflows
* Handling categorical data and class imbalance effectively
* Comparing baseline models before selecting a final model
* Avoiding common runtime and preprocessing errors

---

##   Tools & Libraries

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

---

##   Author

**DHEEPAK G**
Machine Learning | AI | Data Science 

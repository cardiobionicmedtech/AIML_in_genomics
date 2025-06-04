# AML vs. ALL Gene Expression Classification

This repository contains a Jupyter Notebook (**`leukemia_classification.ipynb`**) that performs a comprehensive classification analysis to distinguish **Acute Myeloid Leukemia (AML)** from **Acute Lymphoblastic Leukemia (ALL)** using gene expression profiles.

## 🧠 Project Goal

The primary goal is to build and evaluate machine learning models capable of accurately classifying AML and ALL based on gene expression data. Accurate classification is crucial for determining appropriate treatment strategies for leukemia patients.

## 📊 Dataset

The dataset is sourced from [Kaggle](https://www.kaggle.com/) and includes:

- `data_set_ALL_AML_train.csv`: Training data
- `data_set_ALL_AML_independent.csv`: Independent test data

Each CSV file contains:
- Gene expression levels for multiple patient samples
- Corresponding gene descriptions and accession numbers

## 🔍 Analysis Workflow

1. **Data Loading**: Load both training and independent datasets into pandas DataFrames.
2. **Exploratory Data Analysis (EDA)**: Explore data structure, class distributions, and patterns.
3. **Data Preprocessing**:
   - Clean the data
   - Separate features and target labels
   - Encode the target variable
4. **Feature Selection**:
   - Use `SelectKBest` with `f_classif` to select the top 50 most informative genes.
5. **Model Training & Evaluation**:
   - Train multiple models: Logistic Regression, SVM, Decision Tree, Random Forest, AdaBoost, Gradient Boosting, XGBoost.
   - Evaluate model performance using the independent test set.
6. **Model Comparison & Overfitting Check**:
   - Compare accuracy and performance metrics
   - Assess overfitting by analyzing training vs. test performance
7. **Summary of Findings**

## ✅ Key Findings

- Data was clean with no missing values.
- Class imbalance observed (more ALL than AML cases).
- Top 50 genes were selected as strong features for classification.
- Several models achieved high accuracy (~91%) on the independent dataset.
- Some models showed signs of overfitting, but generalization to the independent test set was still strong.

## 🏆 Best Performing Models

These models achieved the best accuracy (~**0.9118**) on the independent dataset:

- Support Vector Machine (RBF Kernel)
- Decision Tree
- AdaBoost Classifier
- Gradient Boosting Classifier
- XGBoost Classifier

## ⚙️ How to Run

1. Clone this repository.
2. Download the required CSV files from the Kaggle dataset.
   LINK : https://www.kaggle.com/datasets/crawford/gene-expression
4. Upload the files to your working directory or Colab session.
5. Run all cells in `leukemia_classification.ipynb` in sequence.

## 🧩 Dependencies

Install the required libraries using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost


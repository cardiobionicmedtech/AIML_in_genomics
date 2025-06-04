# AIML_in_genomics
# 🔬 AML vs. ALL Gene Expression Classification Using Machine Learning

## 🧾 What is AML and ALL?

**Leukemia** is a type of cancer that affects the blood and bone marrow — the soft tissue inside bones where blood cells are made. Among the various types of leukemia, two major and dangerous subtypes are:

### 🩸 Acute Myeloid Leukemia (AML)
- AML is a **fast-growing** form of blood cancer that starts in the **myeloid cells**, which are responsible for producing red blood cells, white blood cells, and platelets.
- In AML, the bone marrow produces abnormal white blood cells that grow uncontrollably and interfere with the production of normal cells.
- AML is more common in **adults**, especially in older adults, but it can occur at any age.

### 🩸 Acute Lymphoblastic Leukemia (ALL)
- ALL is another **fast-growing** blood cancer, but it starts in the **lymphoid cells**, which form a type of white blood cell called lymphocytes that help fight infection.
- ALL is the **most common type of cancer in children**, but it can also occur in adults.
- Like AML, ALL causes the bone marrow to produce a large number of immature, abnormal white blood cells.

### 😟 Why Is This a Big Problem?
- AML and ALL are **life-threatening conditions** that require **immediate and specific treatment**.
- Despite both being leukemia, **they require entirely different treatments**. Giving the wrong treatment can lead to serious complications or even death.
- Traditional diagnosis requires **bone marrow biopsies, blood tests, genetic analysis, and expert interpretation**, which can be:
  - Time-consuming
  - Expensive
  - Prone to human error in complex cases
- Hence, accurate and early **classification of AML vs. ALL is absolutely critical** to saving lives.

---

## ❗ The Problem This Project Addresses

- Hospitals and labs increasingly collect **gene expression data** — a snapshot of how active thousands of genes are in a patient’s cells.
- This data can help us distinguish between diseases like AML and ALL at a **molecular level**.
- But this data is extremely **large and complex** — a single sample can contain over **7000 gene measurements**.
- It’s **impossible for doctors to manually analyze** this kind of data without help.

---

## 🤖 Why Use AI/ML for Leukemia Classification?

Artificial Intelligence (AI), specifically **Machine Learning (ML)**, can learn patterns from large datasets that are beyond human analysis. For leukemia classification, ML models:

- Learn from thousands of past patient samples
- Automatically discover the most important genes (features)
- Make accurate predictions for new patients
- Save time, cost, and reduce diagnostic errors
- Support doctors in making quicker, more informed decisions

This project applies ML techniques to **automatically classify whether a person has AML or ALL based on gene expression data**, using open-source datasets.

---

## 🎯 Project Objective

To develop and compare machine learning models that can accurately classify whether a patient has **AML or ALL**, based on high-dimensional gene expression profiles.

---

## 📦 Dataset

- **Source**: Publicly available dataset from [Kaggle](https://www.kaggle.com/datasets/crawford/gene-expression)
- **Files Used**:
  - `data_set_ALL_AML_train.csv` – Training samples
  - `data_set_ALL_AML_independent.csv` – Independent test samples

Each row in the dataset represents the gene activity (expression) of a patient, with labels indicating whether the patient has AML or ALL.

---

## 📁 Repository Structure
The project is organized as follows:
```
├── Classification Model for ALL and AML/
│ ├── Classification Model for AML & ALL.ipynb # EDA and classical ML model implementation
│ └── README.md # Detailed information for this section
└── README.md # This main repository README
```


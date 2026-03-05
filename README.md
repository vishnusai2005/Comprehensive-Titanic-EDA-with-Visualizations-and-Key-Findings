# Titanic: Machine Learning from Disaster - Exploratory Data Analysis (EDA)

## Project Overview

This project focuses on a detailed Exploratory Data Analysis (EDA) of the famous Titanic dataset. The goal is to investigate the factors that contributed to a passenger's survival and gain insights through visualization and data cleaning techniques.

## Dataset

The analysis is performed on the standard `train_dataset(1).csv` from the Titanic competition. The dataset contains 891 entries and 12 features, including:

* **Survived:** 0 (No), 1 (Yes)
* **Pclass:** Passenger Class (1, 2, 3)
* **Name, Sex, Age**
* **SibSp:** Number of siblings/spouses aboard
* **Parch:** Number of parents/children aboard
* **Ticket, Fare, Cabin, Embarked**

## Project Files

* `original_titanic_eda.ipynb`: The Jupyter Notebook containing the Python code for the entire EDA process.
* `train_dataset(1).csv`: The dataset used for the analysis.
* `image_abe4c0.png`: The analysis which i was done and i was attached my analysis as an image.

## Key EDA Steps and Methodologies

The EDA process is divided into several sections in the notebook:

### 1. Data Inspection and Understanding
* Checking dimensions (`.shape`) and data types (`.info()`).
* Finding missing values across columns.

### 2. Data Cleaning
* **'Age':** Null values filled with the median to minimize bias from extreme values.
* **'Embarked':** Imputed the missing entries with the most common port (mode).
* **'Cabin':** The entire feature was dropped due to a high percentage of missing values (approx. 77%).
* Confirmed that no more null values exist in the dataset.

### 3. Visualization and Analysis
* We used `seaborn` and `matplotlib` to create visualizations.
* Key functions used:
    * `countplot`: For visualizing distributions of 'Survived', 'Pclass', 'Sex', and 'Embarked'.
    * `histplot`: To analyze numerical features like 'Age' and 'Fare'.
    * `heatmap`: To display a correlation matrix of the features.

## Key Insights and Findings

The analysis revealed significant patterns:

* **Higher Survival for Females:** Females were much more likely to survive (approx. 74%) than males (approx. 19%).
* **Class Matters:** Passenger Class (Pclass) 1 had the highest survival rate, followed by Class 2, and Class 3 had the lowest.
* **Priority for Children:** Children had a higher probability of survival.
* **Age Profile:** The bulk of the passengers fell into the 20-30 age bracket.

## Future Work

* Feature Engineering: Creating new features like 'FamilySize'.
* Machine Learning: building predictive models for survival.
* Advanced visualization for multi-categorical variables.

## Getting Started

To run this project, you will need a Python environment with the following libraries:

```bash
pip install numpy pandas seaborn matplotlib jupyterlab

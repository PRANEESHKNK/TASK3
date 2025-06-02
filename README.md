# 🧠 Bank Marketing Campaign Classification

## 📌 Project Overview
This project implements a Decision Tree Classifier to analyze a dataset related to banking marketing campaigns. The goal is to classify whether a customer will subscribe to a term deposit based on given features.
It uses the [Bank Marketing dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing) from the UCI Machine Learning Repository.

---

## 📊 Dataset Overview

- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)
- **Rows**: 41,188
- **Features**: 20 (both categorical and numerical)
- **Target**: `y` – whether the client subscribed to a term deposit (`yes` or `no`)

---

## 🧼 Preprocessing Steps

- Removed duplicate rows
- Handled missing values (none present)
- Applied **Label Encoding** to all categorical features
- Split the dataset into training and testing sets (70/30 split)

---

## 🤖 Model: Decision Tree 

- **Algorithm**: `sklearn.tree.DecisionTreeClassifier`
- **Criterion**: Gini Index
- **Parameters**:
  - `max_depth=5`
  - `min_samples_split=10`
- Trained on the encoded dataset

---

## ⚙️ Project Workflow
- Data Preprocessing: Cleaning, encoding categorical variables, handling duplicates.
- Train-Test Split: 70% training, 30% testing.
- Model Training: Using DecisionTreeClassifier with gini criterion.
- Evaluation: Checking accuracy on train and test sets.
- Visualization: Plotting the decision tree.


## 🧪 Results

| Metric        | Value      |
|---------------|------------|
| Training Accuracy | ~0.9178086944454081 |
| Testing Accuracy  | ~0.9145146927871772 |

> Note: Replace with actual printed values after running the notebook.

---

## 🌳 Decision Tree Visualization

The decision tree is plotted with all input features, showing splits and class predictions for interpretability.

![Decision Tree Plot](images/decision_tree_plot.png)

---

## 📦 Requirements

```bash
numpy
pandas
matplotlib
seaborn
scikit-learn

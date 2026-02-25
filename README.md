# FindingDonorsProject

# CharityML – Finding Donors

## Overview

This project builds a supervised machine learning model to help CharityML identify potential donors. Based on historical data, all previous donors earned more than $50,000 annually. The goal is to predict whether an individual earns more than $50K in order to reduce mailing costs and increase donation yield.

This is a binary classification problem:

- > 50K → Potential Donor (1)
- <=50K → Not Donor (0)

---

## Workflow

1. **Data Exploration**
   - Analyzed class distribution and dataset balance.

2. **Preprocessing**
   - Log-transformed skewed features (`capital-gain`, `capital-loss`)
   - Scaled numerical features using MinMaxScaler
   - Applied one-hot encoding to categorical variables
   - Encoded target labels as 0 and 1

3. **Modeling**
   - Trained and compared multiple supervised models:
     - Decision Tree
     - Naive Bayes
     - Support Vector Machine
     - Ensemble methods

4. **Evaluation**
   - Used Precision, Recall, and F1 Score
   - Focused on F1 due to class imbalance

5. **Optimization**
   - Tuned the best-performing model using GridSearchCV

---

## Key Takeaways

- Proper preprocessing significantly improves model performance.
- Accuracy alone is not reliable for imbalanced datasets.
- F1 score provides a balanced evaluation of classification performance.
- Ensemble methods perform well on structured tabular data.

---

## Files

- `finding_donors.ipynb` – Main implementation
- `census.csv` – Dataset
- `visuals.py` – Visualization utilities

---

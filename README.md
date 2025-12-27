# Income Classification Using Machine Learning Models
## Overview
This repository presents a comparative analysis of multiple machine learning models applied to a binary income classification task (≤ $50K vs. > $50K). The objective of the project is to evaluate and rank different supervised learning algorithms on non-linearly separable, imbalanced data, and to identify the most effective model based on performance metrics such as accuracy, precision, recall, confusion matrices, and precision–recall (PR) curves.

The **full project report** detailing the methodology, experiments, results, and analysis is available in:
- **`Adult Dataset Report.pdf`**

The **code used to produce the original findings and results** discussed in the report is provided in:
- **`Machine_Learning_Assignment2.ipynb`**

The **Original dataset** used in this project
- **`https://archive.ics.uci.edu/dataset/2/adult`**

## Models Evaluated
The following machine learning models were implemented and analyzed:
- **Decision Tree Classifier**    
- **Support Vector Machine (SVM)** with RBF kernel
- **Neural Networks**    
    - ReLU activation        
    - Hyperbolic tangent activation
- **Logistic Regression**
## Key Findings
### Model Performance Summary
- **Decision Tree** achieved the most balanced performance across accuracy, precision, and recall.
- **Neural Networks** showed competitive accuracy but suffered from low recall, indicating a high number of false negatives.    
- **SVM** achieved the highest recall but had poor precision due to many false positives, reducing its reliability.    
- **Logistic Regression** performed better than expected despite the data violating its linearity and feature independence assumptions.
### Precision–Recall Curve Analysis
- Decision Tree PR curve was closest to the top-right corner, indicating strong overall performance.
- Neural Networks achieved slightly higher AUC values (~0.75) than Decision Tree (~0.70), but curve shape and trade-offs were prioritized over marginal AUC differences.    
- Logistic Regression consistently underperformed in PR analysis.
### Final Model Ranking
Based on the overall analysis, the models ranked as follows:
1. **Decision Tree**
2. **Neural Networks**
3. **Support Vector Machines**
4. **Logistic Regression**

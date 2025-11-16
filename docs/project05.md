# Project 5 – Ensemble Machine Learning (Wine Quality)

This page summarizes my work for Project 5, where I used ensemble models to predict red wine quality.

## Dataset

I used the Red Wine Quality dataset from the UCI Machine Learning Repository.  
The dataset includes 11 input features such as acidity, sugar, density, sulphates, and alcohol.

For this project, I converted the original 0–10 quality score into three categories:

- **0 = low** (quality 3–4)
- **1 = medium** (quality 5–6)
- **2 = high** (quality 7–8)

## Models I Evaluated

I focused on two ensemble models:

### **Random Forest (200, max_depth=10)**  
- Train Accuracy: **0.9758**  
- Test Accuracy: **0.8812**  
- Train F1: **0.9745**  
- Test F1: **0.8596**

### **Gradient Boosting (100)**  
- Train Accuracy: **0.9601**  
- Test Accuracy: **0.8562**  
- Train F1: **0.9584**  
- Test F1: **0.8411**

## Summary

Random Forest had the highest test accuracy and performed the best overall.  
Gradient Boosting was a close second and showed stable results.

For the full notebook, see:  
`notebooks/project05/ensemble-blessing.ipynb`

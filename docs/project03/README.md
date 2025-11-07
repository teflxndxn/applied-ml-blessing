# Project 03
# Project 3 – Building a Classifier (Titanic)

**Author:** Blessing Aganaga  
**Date:** November 2025  

This project builds and evaluates multiple machine learning classification models to predict passenger survival on the Titanic dataset.  
We applied **Decision Tree**, **Support Vector Machine (RBF kernel)**, and **Neural Network (MLP)** models using Scikit-learn.

---

## 🔍 Overview

The goal is to predict whether a passenger survived based on features like:
- Age  
- Sex  
- Fare  
- Family size (engineered feature)  
- Class (`Pclass`)  
- Embarked location  

Each model was trained and tested using a **stratified train/test split** for fairness and reproducibility.

---

## ⚙️ Models Tested

| Model | Key Features Used | Accuracy | Notes |
|-------|--------------------|-----------|-------|
| Decision Tree | alone / age / age + family_size | ~62% | Good interpretability |
| SVM (RBF Kernel) | same cases | ~63% | More stable generalization |
| Neural Network (MLP, scaled) | age + family_size | ~65% | Best overall test accuracy |

---

## 🧩 Key Steps

1. Data cleaning and feature engineering (`family_size`, encoded categorical columns)  
2. Stratified data split for consistent class balance  
3. Model training and evaluation across three feature cases  
4. Generation of confusion matrices and a summary metrics table  
5. Reflection on model performance and improvements  

---

## 📊 Highlights

- Scaling improved both **SVM** and **Neural Network** performance.  
- The **Neural Network (scaled)** achieved the best overall accuracy (~65%).  
- Decision Trees offered interpretability but tended to overfit.  
- “Alone” was a surprisingly strong single predictor of survival.  

---

## 💻 Notebook Link

📘 [Open the full Jupyter notebook here →](../../notebooks/project03/ml03_blessingaganaga.ipynb)

---

## 🧠 Reflection

Using scaled data and richer features improved model performance.  
For deployment, the **Neural Network** or **SVM** would likely generalize better due to their non-linear decision boundaries.

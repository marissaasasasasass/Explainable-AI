# ETDS Assignment 2 — Explainable AI (XAI) for Classification

This repository contains my **Emerging Trends in Data Science (ETDS) Assignment 2** work, focused on building a **classification model** and applying **Explainable AI (XAI)** techniques to explain **why** the model produced its predictions—especially for **5 unseen test samples**.

The dataset is **anonymous** by design to prevent assumptions about feature meaning. The core requirement is not only to achieve reasonable predictive performance, but also to provide **clear, evidence-based explanations** for each test prediction.

---

## Objectives

- Perform data exploration and necessary feature engineering.
- Train an interpretable and/or explainable classification model.
- Achieve reasonably good accuracy (better than random guessing for 2 classes).
- Use at least **one XAI technique** to explain model outcomes.
- Explain the predicted outcomes for **5 unseen test samples** and justify them.
- Include a short self-reflection on what was learned from the module.

---

## What’s Inside

- **Notebook-first submission** (as required):
  - EDA + preprocessing
  - Model training + evaluation
  - XAI explanation section for each of the 5 test samples
  - Reflection section

## Approach (High Level)

### 1) Data Understanding & Preparation
- Inspect dataset structure and missing values
- Handle missing data (imputation or removal where justified)
- Encode categorical features (if any)
- Scale/standardize numeric features when appropriate
- Perform feature selection/engineering only when supported by evidence

### 2) Modeling
- Train one or more classifiers (e.g., logistic regression / tree-based models)
- Validate using train/validation split or cross-validation
- Compare models based on accuracy and stability
- Select a final model for explanation

### 3) Explainable AI (XAI)
At least one XAI technique is applied to explain:
- **Global behavior** (overall feature importance / model tendencies)
- **Local explanations** for each test sample (why this specific outcome)

Examples of XAI methods that may be used:
- Permutation Feature Importance
- SHAP (global + local explanations)
- LIME (local explanations)
- Tree-based feature importance (if using trees)
- Partial Dependence / ICE plots (where applicable)

### 4) Test Sample Explanation (Core Deliverable)
For each of the **5 unseen test samples**, the notebook provides:
- The predicted class
- The top contributing features (direction/magnitude where possible)
- A clear explanation of how the feature values led to that prediction
- Supporting plots/tables from the chosen XAI method(s)

---


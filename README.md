# 🎗️ Breast Cancer Classification with XGBoost

## 💼 Business use case

Predictive models can support diagnostic-review workflows by identifying samples that deserve closer attention. In a clinical context, the useful role is assistance and prioritization—not replacing pathology or medical judgment.

## 🎯 Principal objective

Train an XGBoost classifier on 30 numeric features derived from digitized fine-needle aspirate images and evaluate how well the model separates benign from malignant cases on held-out data.

## 🔎 Summary of takeaways

The saved holdout results report **95.32% accuracy** and **94.16% ROC-AUC**, indicating strong discrimination on the benchmark dataset. XGBoost is a good fit for this kind of structured feature set because it can model nonlinear interactions without requiring a deep-learning pipeline.

For medical decision support, aggregate metrics are not enough. The next review should focus on sensitivity for malignant cases, specificity, calibration, confusion-matrix counts, confidence intervals, and explanation methods such as SHAP. The dataset is also small and curated, so external validation and population-drift analysis would be required before operational use.

## 🧭 Explore the code

The [notebook](https://github.com/saels/breast-cancer-XGBoost-classifier/blob/26cf421ef0e1a8bc0813f1da88cc83eb2a5e9812/Breast_cancer_XGBoost_classifier_.ipynb) covers dataset preparation, XGBoost training, evaluation, and feature importance. Review the implementation for the full modeling flow and the evidence behind the reported benchmark performance.

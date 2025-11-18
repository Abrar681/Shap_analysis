# SHAP Analysis for Survival Models

## 📘 Overview
This project applies **DeepSurv**, a deep learning Cox model, to predict patient survival.  
We use **SHAP** for interpretability (global + local explanations) and compare results with classical **CoxPH**.

## 📂 Repository Structure
- `DeepSurv.ipynb` → Model training & survival curves
- `04_shap_analysis.ipynb` → SHAP global & local analysis
- `results/` → Saved plots and CSVs
- `README.md` → Documentation

## 🎯 Key Deliverables
- DeepSurv survival curves
- SHAP summary plot (global importance)
- SHAP force plots (local patient explanations)
- SHAP vs CoxPH comparison table & scatter plot

## ✅ Conclusion
DeepSurv captures nonlinear survival risk patterns, while SHAP provides transparency.  
Comparison with CoxPH validates consistency between classical and deep survival models.


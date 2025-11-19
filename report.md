# Survival Analysis with DeepSurv and SHAP

## Project Overview
This project implements a survival analysis pipeline using the DeepSurv neural network model. It includes preprocessing, model training, survival curve plotting, and interpretability using SHAP values.

## Objectives
- Predict survival outcomes using DeepSurv.
- Visualize survival curves for different risk groups.
- Interpret model predictions using SHAP (global and local).
- Ensure reproducibility and professional presentation.

## Repository Structure
Shap_analysis/

|-README.md
|-requirements.txt
|-shap_project.py
|-survival_dataset.csv
|-shap_values.csv
|-plot/
* data_distribution.png
* survival_curve.png
* survival by treatment.png
* survivs by gender.png
* survival by comorbidity.png
* Cox Coefficients unpenalized vs penalized.png
* deep surv prediction.png
* shap value impact on model.png
* patient risk.png
* coxph vs shap.png
|-report.md

## Workflow Summary
1. **Data Preparation**  
   - Cleaned and encoded survival dataset.
   - Split into training and test sets.

2. **Modeling with DeepSurv**  
   - Built using PyCox and PyTorch.
   - Trained with early stopping and validation monitoring.

3. **Survival Curve Visualization**  
   - Kaplan-Meier curves for low-risk and high-risk groups.
   - Plots saved in `plot/` folder.

4. **SHAP Interpretability**  
   - Global SHAP summary plot.
   - Local SHAP force plot for individual prediction.
   - SHAP values exported to `shap_values.csv`.

## Reproducibility Notes
- All plots and outputs are saved to `plot/` for easy review.
- Notebook is cleaned of widget metadata to ensure GitHub rendering.
- GitHub token workflow used for secure Colab integration.

## Future Improvements
- Add cross-validation and hyperparameter tuning.
- Extend SHAP analysis to more samples.
- Deploy model with interactive dashboard (e.g., Streamlit).

## Author
**Abrar681**  
Bachelor of Science in Computer Science  
Oracle Cloud Infrastructure Certified  
Currently pursuing AI specialization in machine learning  
GitHub: [github.com/Abrar681](https://github.com/Abrar681)


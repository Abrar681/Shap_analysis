# SHAP Analysis for Survival Models

## 📘 Overview
This project applies **DeepSurv**, a deep learning Cox model, to predict patient survival.  
We use **SHAP** for interpretability (global + local explanations) and compare results with classical **CoxPH**.

Survival-SHAP-Project/
│
├── shap_analysis.ipynb              
├── survival_dataset.csv             
├── shap_values.csv                  
├── plot/                            
│   |-- data_distribution.png        
│   |-- survival_curve.png           
│   |-- survival by treatment.png                 
│   |-- survivs by gender.png             
│   |-- survival by comorbidity.png        
│   |-- Cox Coefficients unpenalized vs penalized.png
|   |-- deep surv prediction.png
|   |-- shap value impact on model.png
|   |-- patient risk.png
|   |-- coxph vs shap.png
├── report.md                      
├── requirements.txt               
└── README.md                      


Project Workflow
----------------
1️⃣ Data Loading & Preprocessing
Loads the survival_dataset.csv file

Handles missing values

Encodes categorical variables

Splits data into train/test sets

Scales features for neural network training

Saves distribution plot to plot/data_distribution.png

2️⃣ Model Training
-----------------
A DeepSurv-style CoxPH model (PyCox + PyTorch) is trained to predict survival outcomes.

3️⃣ Model Evaluation
--------------------
The notebook reports key survival metrics:

Concordance index (C-index)

Kaplan–Meier baseline curve

DeepSurv survival curves for test samples

All plots saved to plot/ folder

4️⃣ Explainability with SHAP
----------------------------
SHAP is used to provide interpretability:

🔹 Global Interpretability
shap_summary.png

Shows the most important features affecting survival predictions

Highlights direction and magnitude of influence

🔹 Local Interpretability
shap_force_plot.html

Explains individual survival prediction

Useful for fairness and clinical transparency

shap_dependence.png

Shows how one feature interacts with others

Outputs
-------
* data_distribution plot      
* survival_curve plot           
* survival by treatment plot                 
* survivs by gender plot             
* survival by comorbidity plot        
* Cox Coefficients unpenalized vs penalized plot
* deep surv prediction plot
* shap value impact on model plot
* patient risk plot
* coxph vs shap plot
* shape_values.csv

 Purpose of the Project
-----------------------
This project demonstrates:

* How DeepSurv-style survival models operate
* How explainability tools (SHAP) help interpret survival predictions
* How to identify important risk factors influencing survival outcomes
* How to justify model decisions to stakeholders in healthcare or research

How to Run
----------
Install required dependencies:
bash
pip install -r requirements.txt

Open the notebook:
-----------------
Code
shap_analysis.ipynb

Additional Documentation
------------------------
See report.md for:

* Full interpretation of results
* Explanation of SHAP values
* Strengths & limitations of the model
* Recommendations for improvement

Author
Abrar shaukathali
GitHub: https://github.com/Abrar681

Conclusion
----------
DeepSurv captures nonlinear survival risk patterns, while SHAP provides transparency.  
Comparison with CoxPH validates consistency between classical and deep survival models.


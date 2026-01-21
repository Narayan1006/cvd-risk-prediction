🫀 Interpretable CVD Risk Prediction

An interpretable machine learning approach for early cardiovascular disease (CVD) risk prediction and clinical risk stratification using routine health data.

📌 Overview

Cardiovascular disease remains the leading cause of death globally. Early identification of high-risk individuals enables preventive interventions and better clinical outcomes.
This project builds an explainable machine learning pipeline that predicts cardiovascular disease risk and translates predictions into clinically meaningful risk categories.

The focus is not only on accuracy, but also on interpretability, transparency, and real-world usability.

🎯 Objectives

Predict the presence of cardiovascular disease using clinical features

Maintain high recall for high-risk patients

Provide transparent explanations using feature importance and SHAP

Convert model outputs into low, moderate, and high risk groups

📊 Dataset

De-identified cardiovascular health dataset

Includes demographic, physiological, exercise-related, and ECG features

Target variable: HeartDisease (0 = No, 1 = Yes)

Dataset is preprocessed and encoded for direct use in ML models

🧠 Methodology

Exploratory Data Analysis (EDA)

Feature correlations

Age vs heart disease analysis

Modeling

Logistic Regression (baseline, interpretable)

Random Forest (final model, non-linear interactions)

Evaluation Metrics

Accuracy

ROC-AUC

Precision, Recall, F1-score

Emphasis on minimizing false negatives

Interpretability

Random Forest feature importance

SHAP (SHapley Additive exPlanations) for global explanation

Risk Stratification

Low Risk

Moderate Risk

High Risk

📈 Results

Random Forest ROC-AUC: ~0.94

High recall (~93%) for patients with heart disease

Most influential features:

ST Depression (Oldpeak)

ST Slope abnormalities

Exercise-induced angina

Maximum heart rate

Age

Risk stratification revealed clinically consistent patterns across patient groups.

🏥 Clinical Relevance

The system is designed as a decision-support tool, not a diagnostic replacement.
It can assist:

Primary care screening

Community health programs

Preventive cardiovascular risk assessment

Especially valuable in low-resource settings where specialist access is limited.

⚠️ Limitations

Trained on a single dataset

No external validation yet

Not intended to replace medical judgment

🔮 Future Work

External validation on diverse populations

Longitudinal risk progression modeling

Fairness and bias analysis across demographics

Deployment as a lightweight clinical decision-support application

🧰 Built With

Python

Pandas

NumPy

Scikit-learn

SHAP

Matplotlib

Seaborn

Google Colab

▶️ How to Run

Open the notebook:
Interpretable_CVD_Risk_Prediction.ipynb

Run all cells from top to bottom

Ensure required Python libraries are installed

📄 License

This project is for educational and research purposes only.

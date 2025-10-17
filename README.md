Breast Cancer Prognosis Prediction
Overview
This notebook predicts breast cancer prognosis (whether a patient survives or not) using gene expression data.
It uses a public dataset from GEO (GSE20685) and applies machine learning to identify which genes are most linked to poor outcomes.
Steps in the Notebook
Load Dataset – Downloads the gene expression data and patient information (death event).
Clean Data – Removes missing values and matches expression data with survival info.
Normalize Features – Scales all gene values for fair model training.
Select Important Genes – Picks top 1,000 genes that best separate survived vs. died patients.
Train Models – Uses Logistic Regression, Random Forest, and SVM to classify prognosis.
Evaluate Models – Measures model accuracy using AUC (Area Under Curve) to see how well the model distinguishes high- and low-risk patients.
What It Shows
Certain genes have expression patterns that differ between patients who survive and those who don’t.
The models can use these gene patterns to predict prognosis (good vs. poor outcome).
A higher AUC value means the model predicts prognosis more accurately.
Output
Class balance (how many survived vs. died).
Number of features used after selection.
Cross-validation AUC scores for each model.
Tech Stack
Python
scikit-learn, pandas, numpy, matplotlib, seaborn

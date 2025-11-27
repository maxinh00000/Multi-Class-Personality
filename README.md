# Multi-Class-Personality
Multiclass classification model to predict personality clusters using behavioral/lifestyle features.
📁 Repository Structure
Multi-Class-Personality/
│
├── train.csv                     # Training data (features + target)
├── test.csv                      # Test data (features only)
├── sample_submission.csv         # Format for predictions
│
├── multi.ipynb                   # Main notebook: EDA, preprocessing, modeling, ensembling
│
├── ensemble_submission.csv       # Submission file (model ensemble)
├── d_ensemble_submission.csv
├── newensemble_submission.csv
│
└── README.md                     # Project documentation

Approach & Methodology
1️⃣ Exploratory Data Analysis

Checked distributions and missing values

Visualized correlations

Identified class imbalance

2️⃣ Data Preprocessing

Filled missing values

Encoded categorical variables

Scaled numerical features

3️⃣ Modeling

Multiple algorithms were trained and compared:

SVM

MLP

Logistic Regression

Random Forest

XGBoost



4️⃣ Ensembling

Final predictions were generated using:

Soft Voting Ensemble

Weighted averaging

Experimentation on multiple ensemble variants

5️⃣ Evaluation

Primary metric:

Macro F1 Score

Macro F1 treats all classes equally, which is essential because some personality clusters appear less frequently.

Final Output

Model predictions are saved as CSV files in the format:

id,personality_cluster
0,Cluster_1
1,Cluster_4
2,Cluster_2
.

Install dependencies
pip install -r requirements.txt

Run the notebook
jupyter notebook multi.ipynb



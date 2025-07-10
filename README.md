📊 Predicting Term Deposit Subscriptions Using Machine Learning:

This project uses various machine learning models to predict whether a customer will subscribe to a term deposit based on data from direct marketing campaigns conducted by a Portuguese banking institution.




Author: Rajiv Puli
University: Kansas State University
Course: Machine Learning (Fall 2021)





📁 Project Overview:

Financial institutions rely on term deposits to generate capital. By using customer and campaign data, this project builds and evaluates multiple classification models to predict whether a client will subscribe to a term deposit (y = 1) or not (y = 0). The best-performing model, XGBoost, achieved an accuracy of 89%.





📌 Problem Statement:

Objective: Predict the outcome (y) of a term deposit marketing campaign.

Target Variable: y (1 = Subscribed, 0 = Not Subscribed)







📊 Dataset:


Source: UCI Machine Learning Repository

Records: 45,211

Features: 17 (numerical & categorical)

File Size: ~10 MB

Context: Direct phone marketing campaign data from a Portuguese bank.







🧹 Data Preprocessing:

No missing values.

Binary categorical values (yes/no) were converted to 1/0.

Feature engineering performed using ExtraTreesClassifier.

5 unimportant features were removed, but model performance did not improve.








📈 Exploratory Data Analysis:

Bar charts and heatmaps revealed a strong positive correlation between duration and y.

Imbalance in subscription rates was addressed via cross-validation rather than resampling.








🤖 Machine Learning Models Used and Their Accuracy:

Decision Tree	85%
Random Forest	~87%
Logistic Regression	~86%
Naive Bayes	~83%
K-Nearest Neighbors	~84%
Support Vector Machine	~85%
XGBoost	89%


K-Fold Cross Validation (k=10) was used for all models.

XGBoost showed the best ROC-AUC and overall performance.









🧪 Evaluation Metrics:


Accuracy

Precision

Recall

F1-Score

ROC-AUC Curve

XGBoost showed a 4% improvement in accuracy over the baseline (Decision Tree).








🛠️ Tools & Technologies:


Python (Jupyter Notebook)

Libraries: scikit-learn, pandas, matplotlib, numpy, xgboost








🔭 Future Work:


Improve accuracy via advanced feature engineering.

Experiment with deep learning models (e.g., PyTorch).

Apply the pipeline to larger or similar financial datasets.









📚 References:

Moro, S., Cortez, P., & Rita, P. (2014). A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier.

Moro, S., Laureano, R., & Cortez, P. (2011). Using Data Mining for Bank Direct Marketing: An Application of the CRISP-DM Methodology. ESM 2011, EUROSIS.








📎 Project Files:


Final Report Machine Learning.pdf – Full written report

Final Project Machine Learning.pptx – Presentation slides

notebook.ipynb – Jupyter Notebook (add to repo)

data.csv – Dataset (link or include if license allows)


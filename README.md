# Teen-Phone-Addictio-

Phone Addiction Prediction Among Teens
📌 Project Overview

This project analyzes a dataset of teenage smartphone users to predict their phone addiction level based on lifestyle, behavioral, and psychological factors. It uses both regression to predict numeric addiction scores and classification to categorize addiction into Low, Medium, and High.

🎯 Problem Statement

With growing smartphone usage among teenagers, early detection of problematic behavior can help parents and educators intervene.
This project uses machine learning to predict phone addiction severity and understand the factors contributing to it.

📁 Dataset
📂 File: teen_phone_addiction_dataset.csv

👥 Variables include:

Daily_Usage_Hours, Sleep_Hours, Screen_Time_Before_Bed

Social_Interactions, Anxiety_Level, Depression_Level

Phone_Usage_Purpose, Academic_Performance, Parental_Control

🧰 Tools & Technologies Used
Python (Pandas, NumPy)

Seaborn & Matplotlib – Visualizations

Scikit-learn – Regression & Classification Models

Jupyter / Colab Notebook

🔍 Exploratory Data Analysis
Key visualizations included:

Correlation heatmaps for behavioral & psychological features

Distribution of Addiction_Level

Bar charts for age and gender-based trends

Scatter plots of usage vs addiction

Pair plots across critical features

📐 Feature Engineering
Dropped irrelevant fields (e.g., Name, ID, School_Grade)

Created a new feature Addiction_Class using binning:

0–4 → Low

5–7 → Medium

8–10 → High

Encoded categorical features (Gender, Phone_Usage_Purpose) using LabelEncoder

🤖 Machine Learning Models
🔹 Regression – Predict Addiction_Level (0–10 scale)
Metric	Value
R² Score	0.45
MAE	value may vary depending on fix
MSE	value may vary depending on fix

📌 Note: Ensure Addiction_Level is treated as a numeric target without label encoding.

🔹 Classification – Predict Addiction_Class (Low/Medium/High)
Model: RandomForestClassifier

Metric	Score
Accuracy	~84%
Precision	Reported
Recall	Reported
F1 Score	Reported

📊 Also included: Confusion matrix + classification report

📈 Feature Importance (Random Forest)
Daily_Usage_Hours, Sleep_Hours, Screen_Time_Before_Bed were among the top predictors.

Depression_Level and Social_Interactions also influenced predictions.

🧠 Key Insights
Teens with higher daily usage tend to have higher addiction scores.

Less sleep is strongly associated with higher phone addiction.

Social media is the most common usage purpose.

Ages 15–17 showed the highest average addiction levels.

Parental control had weak correlation with actual addiction.

🧾 Project Structure
lua
Copy
Edit
|-- phone_addiction_project/
|   |-- teen_phone_addiction_dataset.csv
|   |-- phone_addiction_modeling.ipynb
|   |-- phone_addiction.py
|   |-- README.md
|   |-- visualizations/
🚀 Future Improvements
Use OneHotEncoding instead of LabelEncoding for categorical features

Tune hyperparameters in Random Forest

Deploy the model with Streamlit

# Spotify

# 🎧 Spotify Churn Prediction Project
## 📄 Overview

This project explores customer churn prediction for a simulated Spotify dataset using machine learning models.
The notebook (spotfy.ipynb) includes data exploration, feature engineering, visualization, and classification modeling to predict whether a user will churn or stay active.

## 🧠 Objectives

Understand user behavior patterns such as listening time, device type, and subscription level.

Identify key features that influence churn.

Build and evaluate machine learning models to predict churn.

## 📊 Dataset Information

Rows: 8000

Columns: 12

Target variable: is_churned

Key Features:

gender, age, country, subscription_type, listening_time,

songs_played_per_day, skip_rate, device_type,

ads_listened_per_week, offline_listening

No missing or duplicate values were found.

## 🧩 Exploratory Data Analysis (EDA)

The notebook includes:

Gender and subscription-type distribution

Average listening time

Correlation heatmap of numeric features

Country-level user counts

Example Visuals:

sns.heatmap() for feature correlation

matplotlib bar and pie charts for demographic distributions

## ⚙️ Model Development

Two models were implemented:

Decision Tree Classifier

Random Forest Classifier

The features were scaled using StandardScaler, and the dataset was split using train_test_split.

## 📈 Model Performance
Model	Accuracy	Precision	Recall	Notes
Decision Tree	0.6169	0.2777	0.3325	Decent balance but weak recall
Random Forest	0.7406	0.2581	0.0200	High accuracy but biased toward majority class

Both models show class imbalance, performing better at predicting non-churned users.

## 🔢 Confusion Matrices

Decision Tree:

[[854 346]
 [267 133]]


Random Forest:

[[1177   23]
 [ 392    8]]


Visualization:

sns.heatmap(confusion_matrix, annot=True, cmap='Blues', fmt='d')
plt.title('Confusion Matrix')
plt.xlabel('Predicted')
plt.ylabel('Actual')
plt.show()

## 🧰 Tools and Libraries

Python 3.x

pandas, numpy

matplotlib, seaborn

scikit-learn

## 🚀 How to Run

Clone the repository:

git clone https://github.com/<your-username>/spotify-churn-prediction.git


Install dependencies:

pip install -r requirements.txt


Open the notebook:

jupyter notebook spotfy.ipynb


Or open directly in a new window via Google Colab
 (enable pop-ups if blocked).

## 💡 Future Improvements

Address class imbalance using SMOTE or class weights.

Experiment with XGBoost or Logistic Regression.

Perform hyperparameter tuning to improve recall and precision.

## 📬 Author

John Mwangi
Data Analyst & ML Enthusiast

📧 Connect on linkedin(https://www.linkedin.com/in/john-m-mwangi/)

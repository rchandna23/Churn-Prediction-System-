# Churn-Prediction-System-
A machine learning–based Customer Churn Prediction System that identifies customers likely to leave a service using behavioral and demographic data. Built with Random Forest Classifier and deployed on AWS Cloud, it enables businesses to take proactive retention measures through accurate and scalable predictions.
🧠 Customer Churn Prediction System using AWS Cloud & Machine Learning
📘 Overview

The Customer Churn Prediction System is a machine learning project designed to identify customers who are likely to discontinue a service or subscription.
This system leverages AWS Cloud Services for deployment and scalability, and applies the Random Forest Classifier for accurate churn prediction.

The goal is to help businesses make data-driven decisions to improve customer retention and reduce churn rate.

🚀 Key Features

📊 Machine Learning Model: Uses Random Forest Classifier for robust prediction.

☁️ AWS Cloud Integration: Model hosted and deployed using AWS S3, EC2, and Lambda.

📈 Interactive Dashboard: Visualize churn metrics using Power BI or Streamlit (optional).

🔍 Feature Importance Analysis: Understand which customer attributes contribute most to churn.

🧩 End-to-End Pipeline: From data preprocessing → model training → prediction → deployment.

🏗️ System Architecture
Data Source → Data Preprocessing → Feature Engineering → Model Training → Model Evaluation → AWS Deployment → Prediction API
🧰 Tech Stack

Category	Tools & Technologies

Programming Language	Python 3.x
ML Framework	scikit-learn, pandas, numpy
Cloud Services	AWS S3, AWS EC2, AWS Lambda, AWS SageMaker (optional)
Data Visualization	Power BI / Matplotlib / Seaborn
Version Control	Git & GitHub
Deployment	Flask API + AWS Lambda / EC2
Storage	Amazon S3 Bucket

⚙️ Setup & Installation
1️⃣ Clone the Repository
git clone https://github.com/yourusername/Churn-Prediction-System.git
cd Churn-Prediction-System
2️⃣ Create a Virtual Environment
python -m venv venv
source venv/bin/activate   # for Mac/Linux
venv\Scripts\activate      # for Windows
3️⃣ Install Dependencies
pip install -r requirements.txt
☁️ AWS Cloud Deployment
Steps:

Upload trained model (random_forest_model.pkl) to AWS S3.
Deploy API using AWS Lambda and API Gateway.
Optionally, use AWS EC2 or SageMaker for large-scale model training.
Configure IAM roles for secure access to S3 and Lambda.

🧪 Model Details
Algorithm: Random Forest Classifier
Reason for Selection:
Handles both categorical & numerical data efficiently.
Resistant to overfitting compared to decision trees.
Provides high accuracy and feature importance insights.

Metrics
Metric	Score
Accuracy	0.83
Precision	0.81
Recall	0.79
F1-Score	0.80
📊 Example Prediction

Input (JSON):

{
  "gender": "Female",
  "SeniorCitizen": 0,
  "Partner": "Yes",
  "MonthlyCharges": 70.35,
  "tenure": 12
}

Output:

{
  "churn_prediction": "Yes",
  "confidence_score": 0.82
}
📈 Future Enhancements

Integrate Deep Learning models (XGBoost, LSTM).

Build a Streamlit dashboard for live churn monitoring.

Add AWS SageMaker pipeline automation.

Enable real-time API inference for CRM integration.

🤝 Contributors

Rachit Chandna 
Hashmat Aziz Rather

📜 License
This project is licensed under the MIT License — feel free to use and modify with attribution.

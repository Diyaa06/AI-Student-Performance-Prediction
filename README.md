AI-Based Student Performance Prediction
Overview

The AI-Based Student Performance Prediction project is an end-to-end Machine Learning solution designed to predict students' academic performance and identify those who may be at risk of poor outcomes. The project leverages regression, classification, deep learning, and reinforcement learning techniques to analyze academic and behavioral factors, enabling data-driven educational insights.

The primary objective is to assist educational institutions in monitoring student performance, detecting learning risks at an early stage, and supporting timely academic interventions.

Problem Statement

Student performance is influenced by multiple academic and behavioral factors, making early identification of struggling students a challenging task. Traditional evaluation methods often detect issues only after examinations, leaving limited opportunities for intervention.

This project addresses the problem by building predictive models capable of:

Estimating students' final academic scores.
Identifying students who require academic support.
Discovering hidden relationships between academic features.
Supporting data-driven decision making for educators.
Objectives
Predict students' final scores using regression techniques.
Classify students as academically at-risk or not at-risk.
Compare multiple Machine Learning algorithms.
Improve prediction accuracy through feature engineering and preprocessing.
Explore Deep Learning and Reinforcement Learning approaches for educational analytics.
Dataset

The dataset contains academic and behavioral attributes of students, including:

Mathematics Score
Statistics Score
Python Score
Machine Learning Quiz Score
Deep Learning Quiz Score
Attendance
Study Hours
Sleep Hours
Stress Level
Previous Experience
Branch
Target Variables
Final Score (Regression)
At Risk (Binary Classification)
Project Workflow
Data Collection
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Data Preprocessing
        │
        ▼
Feature Engineering
        │
        ▼
Model Training
        │
        ├── Regression
        ├── Classification
        ├── Deep Learning
        └── Reinforcement Learning
        │
        ▼
Model Evaluation
        │
        ▼
Prediction & Submission
Exploratory Data Analysis

The dataset was analyzed to understand its structure and identify meaningful relationships before model development.

The analysis included:

Missing value analysis
Duplicate record detection
Statistical summary
Feature distribution
Correlation analysis
Attendance analysis
Study hours analysis
Final score distribution
Risk distribution
Branch-wise comparison
Data Preprocessing

Several preprocessing techniques were applied to improve model performance and data quality.

Missing value imputation
Outlier treatment
Label Encoding
Feature Scaling
Feature Engineering
Log Transformation
Interaction Feature Creation
Derived Statistical Features
Models Used
1. Ridge Regression

Ridge Regression was used as the baseline regression model to understand the linear relationship between academic features and student performance while reducing overfitting through L2 regularization.

2. Random Forest Regressor

Random Forest Regressor was implemented to capture complex and non-linear relationships among academic variables. Its ensemble learning approach improves robustness and generalization.

3. XGBoost Regressor

XGBoost was evaluated due to its ability to model complex feature interactions efficiently while achieving strong predictive performance on structured datasets.

4. Deep Learning (Multi-Layer Perceptron)

A Multi-Layer Perceptron (MLP) neural network was developed to automatically learn hidden relationships among academic and behavioral features.

The architecture consists of multiple dense layers with ReLU activation, Dropout regularization, and Adam optimization.

Among all regression models, the MLP achieved the best predictive performance.

5. Random Forest Classifier

Random Forest Classifier was used to identify students who are academically at risk.

Class balancing techniques were applied, and the model was evaluated using the F1-score, which provides a better assessment for imbalanced datasets.

6. Reinforcement Learning (Q-Learning)

A Q-Learning agent was implemented to simulate an intelligent tutor allocation strategy.

The model learns the optimal tutoring policy by interacting with the environment and maximizing cumulative learning rewards.

Model Performance
Regression
Model	RMSE
Ridge Regression	4.88
Random Forest	5.22
XGBoost	5.17
Deep Learning (MLP)	4.73

Best Performing Model: Deep Learning (MLP)

Classification
Model	F1 Score
Random Forest Classifier	0.556
Reinforcement Learning
Model	Average Reward
Baseline Policy	388.19
Q-Learning	404.25

The Q-Learning agent achieved higher cumulative rewards than the baseline strategy.

Technologies Used
Programming Language
Python
Libraries
NumPy
Pandas
Matplotlib
Seaborn
Scikit-learn
TensorFlow / Keras
XGBoost
Development Environment
Jupyter Notebook
Kaggle Notebook
Repository Structure
AI-Student-Performance-Prediction/
│
├── notebook.ipynb
├── train.csv
├── test.csv
├── sample_submission.csv
├── submission.csv
├── README.md
└── requirements.txt
Future Enhancements
Deploy the prediction model as a web application.
Integrate real-time student performance monitoring.
Improve classification accuracy through hyperparameter optimization.
Explore ensemble learning and transformer-based architectures.
Develop an interactive dashboard for educators.
Conclusion

This project demonstrates the application of Machine Learning, Deep Learning, and Reinforcement Learning techniques to solve a real-world educational problem. By combining predictive analytics with feature engineering and model comparison, the system provides meaningful insights into student performance and supports proactive academic decision-making.

Author

Aparupa Samal

B.Tech – Computer Science Engineering (Artificial Intelligence & Machine Learning)

Parul Institute of Engineering & Technology, Parul University

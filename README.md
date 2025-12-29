Intelligent Resource Allocation Predictor (OS + Machine Learning)
📌 Project Overview

Modern operating systems allocate CPU and memory reactively, responding only after load increases.
This project proposes an intelligent, proactive resource allocation system that uses machine learning to predict future system load and recommend optimal resource allocation decisions before overload occurs.

The system integrates Operating System concepts with Regression, Classification, and Time-Series forecasting to analyze real-time system metrics and assist in intelligent scheduling decisions.

🎯 Objectives

Collect real-time OS performance metrics

Perform feature engineering on system-level data

Predict future CPU usage using regression

Classify workload intensity using classification

Forecast future trends using time-series analysis

Provide intelligent resource allocation recommendations

🧠 Core Concepts Used

Operating Systems (CPU scheduling, memory utilization)

Machine Learning (Regression & Classification)

Time Series Forecasting (ARIMA)

Feature Engineering

Predictive Analytics

Proactive Resource Management

🏗️ System Architecture
System Metrics (CPU, Memory, Disk)
        ↓
Data Collection (psutil)
        ↓
Feature Engineering
        ↓
ML Models
  ├── Regression (CPU Prediction)
  ├── Classification (Workload Type)
  └── Time Series Forecasting
        ↓
Intelligent Resource Recommendation

🛠️ Technology Stack

Language: Python

Libraries:

psutil

pandas

numpy

scikit-learn

statsmodels

joblib

Tools:

VS Code

GitHub

📁 Project Structure
Intelligent-Resource-Allocation-Predictor/
│
├── data/
│   ├── system_metrics.csv
│   └── processed_metrics.csv
│
├── models/
│   ├── cpu_regressor.pkl
│   └── workload_classifier.pkl
│
├── src/
│   ├── data_collector.py
│   ├── feature_engineering.py
│   ├── train_regression.py
│   ├── train_classifier.py
│   ├── time_series_forecast.py
│   └── predictor.py
│
├── requirements.txt
├── README.md
└── .gitignore

⚙️ How the System Works
1️⃣ Data Collection

Collects real-time CPU, memory, and disk usage using psutil

Labels workload as Light / Medium / Heavy

2️⃣ Feature Engineering

Creates derived features such as CPU–memory interaction ratios

Improves learning efficiency of ML models

3️⃣ Regression Model

Predicts future CPU usage

Helps estimate upcoming resource demand

4️⃣ Classification Model

Classifies workload intensity

Enables policy-based resource decisions

5️⃣ Time-Series Forecasting

Uses ARIMA to predict CPU trends over time

Enables proactive scheduling

6️⃣ Intelligent Predictor

Combines all models

Outputs real-time recommendation for resource allocation

▶️ How to Run the Project
1. Clone the repository
git clone https://github.com/your-username/Intelligent-Resource-Allocation-Predictor.git
cd Intelligent-Resource-Allocation-Predictor

2. Create and activate virtual environment
python -m venv venv
venv\Scripts\activate

3. Install dependencies
pip install -r requirements.txt

4. Run step-by-step
python src/data_collector.py
python src/feature_engineering.py
python src/train_regression.py
python src/train_classifier.py
python src/time_series_forecast.py
python src/predictor.py

📊 Sample Output
===== INTELLIGENT RESOURCE ALLOCATION PREDICTOR =====

Current CPU Usage      : 34.20%
Current Memory Usage   : 62.10%
Current Disk Usage     : 45.00%

Predicted CPU Usage    : 38.45%
Workload Classification: Medium

Recommendation: Maintain BALANCED resource allocation.

💡 Key Highlights

Uses real OS metrics, not synthetic data

Combines multiple ML paradigms

OS-aware decision-making

Modular and extensible design

Industry-relevant problem statement

🧪 Possible Enhancements

Integrate with OS schedulers

Add cloud workload datasets

Implement reinforcement learning

Visualize metrics using dashboards

Extend to distributed systems

🎓 Academic & Interview Relevance

This project demonstrates:

Strong understanding of Operating Systems

Practical application of Machine Learning

Real-world system design thinking

Predictive and proactive optimization techniques

👤 Author

Khadijah Mujibir Rahiman
B.E. Computer Science and Engineering
St. Joseph’s Institute of Technology



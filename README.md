# Student Performance Prediction

An end-to-end machine-learning web application that predicts student exam scores and visualizes performance drivers.  
Built with a Flask front end, a trained CatBoost model, and production-ready CI/CD and MLOps workflows.

---

## 🚀 Features

- **Predictive Model**  
  - Trained a CatBoost regressor on student demographics and academic features.  
  - Achieved an R² of 0.85 on the hold-out test set.
- **Interactive Web App**  
  - Flask app exposing a `/predict` API and a simple HTML UI for live predictions.
- **Experiment Tracking**  
  - MLflow tracks experiments, parameters, metrics, and model artifacts.
- **CI/CD with GitHub Actions**  
  - Pipeline runs linting, unit tests, model training, and Docker image build on every push to `main`.
- **Containerization & Deployment**  
  - Docker image pushed to AWS ECR.  
  - Application deployed on AWS ECS Fargate.  
  - EC2 hosts auxiliary services (logging, monitoring).

---

## 🛠 Tech Stack

- **Languages & Frameworks:** Python, Flask, Jinja2  
- **ML & Tracking:** CatBoost, MLflow  
- **CI/CD:** GitHub Actions  
- **Containerization:** Docker, AWS ECR, AWS ECS Fargate  
- **Hosting:** AWS EC2 (backend services)  
- **Data Storage:** Local CSVs / SQLite for demo

---

## 📥 Getting Started

1. **Clone & Install**  
   ```bash
   git clone https://github.com/Venkat450/student-performance.git
   cd student-performance
   pip install -r requirements.txt

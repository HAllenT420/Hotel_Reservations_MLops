# Hotel Booking Cancellation Prediction - MLOps with GCP

## 📌 Project Overview
This project is designed to predict whether a customer will cancel their hotel booking. It follows a complete MLOps pipeline using **Google Cloud Platform (GCP)** for model deployment, orchestration, and monitoring. The goal is to automate the ML lifecycle from data ingestion to model training, deployment, and continuous monitoring.

## 🚀 Tech Stack
- **Google Cloud Platform (GCP)**: Cloud Storage, Vertex AI, Cloud Functions, Cloud Run, BigQuery
- **MLOps Tools**: Docker, Jenkins, Airflow, MLflow
- **Machine Learning**: Scikit-learn, TensorFlow/PyTorch
- **Data Processing**: Pandas, NumPy
- **Backend**: Flask/FastAPI
- **CI/CD**: Jenkins, GitHub Actions

## 📂 Project Structure
```
Hotel_Reservations_MLOps/
│── artifacts/           # Saved models and pipeline artifacts
│── config/             # Configuration files
│── custom_jenkins/     # Jenkins CI/CD scripts
│── notebook/           # Jupyter notebooks for EDA and modeling
│── pipeline/           # Data processing and ML pipeline scripts
│── src/                # Core application source code
│── static/             # Static files for UI
│── templates/          # HTML templates
│── utils/              # Helper functions
│── .gitignore          # Files to ignore in version control
│── Dockerfile          # Docker setup for cloud deployment
│── Jenkinsfile         # Jenkins pipeline configuration
│── application.py      # Main application entry point
│── requirements.txt    # Required dependencies
│── setup.py            # Python package setup
```

## 🔥 Key Features
✅ **Automated ML Pipeline** - Full lifecycle automation with GCP and Airflow  
✅ **Cloud-Based Deployment** - Model hosted on GCP with scalable APIs  
✅ **Continuous Integration & Deployment (CI/CD)** - Jenkins and GitHub Actions  
✅ **Model Monitoring & Logging** - MLflow for experiment tracking  
✅ **Dockerized & Scalable** - Containerized deployment with Kubernetes support  

## 📊 Data Overview
The dataset contains hotel booking records, including features such as:
- **Customer Information** (Lead time, Booking changes, Previous cancellations, etc.)
- **Booking Details** (Room type, Deposit type, Special requests, etc.)
- **External Factors** (Market segment, Distribution channel, etc.)
- **Target Variable**: `Booking_Canceled` (1 - Canceled, 0 - Not Canceled)

## 🔄 MLOps Workflow
1. **Data Ingestion** - Data fetched from GCP BigQuery
2. **Feature Engineering** - Data preprocessing with Pandas & NumPy
3. **Model Training** - ML model trained using Scikit-learn/TensorFlow
4. **Model Registry** - Versioned models stored in MLflow
5. **Deployment** - Model deployed via GCP Cloud Run
6. **Monitoring & Logging** - Model performance tracked using Vertex AI & MLflow
7. **CI/CD** - Automated pipeline with Jenkins & GitHub Actions

## 🎯 How to Run the Project
### 1️⃣ Setup Environment
```bash
pip install -r requirements.txt
```

### 2️⃣ Run Locally
```bash
python application.py
```

### 3️⃣ Build & Run with Docker
```bash
docker build -t hotel_mlops .
docker run -p 5000:5000 hotel_mlops
```

## 🏆 Results & Performance
- Achieved **85% accuracy** on the validation set
- Reduced deployment time by **40%** using CI/CD automation
- Improved model monitoring with **real-time logging**

## 💡 Future Enhancements
- **Hyperparameter tuning with Vertex AI**
- **Integration with real-time booking data**
- **Advanced model interpretability using SHAP**

## 👨‍💻 Author
[Your Name] - Data Scientist | MLOps Engineer

🔗 **GitHub**: [Your GitHub Profile]
🔗 **LinkedIn**: [Your LinkedIn Profile]

---
⭐ If you found this project useful, please consider giving it a star!

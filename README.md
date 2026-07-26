# 🐳 Student Health Risk Prediction - Docker Deployment

A Dockerized deployment of the Student Health Risk Prediction application built using **FastAPI**, **Streamlit**, and **CatBoost**.

This repository demonstrates how to package a machine learning application into Docker containers, publish them to Docker Hub, and prepare them for deployment on cloud platforms such as AWS EC2.

---

# 🚀 Features

- Dockerized FastAPI backend
- Dockerized Streamlit frontend
- REST API for predictions
- Interactive web interface
- Pre-trained CatBoost model
- Ready for AWS EC2 deployment
- Docker Hub published images

---

# 🏗️ Project Architecture

```
Browser
    │
    ▼
Streamlit Frontend
    │
    ▼
FastAPI Backend
    │
    ▼
CatBoost Model
```

---

# 📁 Project Structure

```
STUDENT_HEALTH_DOCKER/
│
├── api/
│   └── app.py
│
├── frontend/
│   └── app.py
│
├── model/
│   └── model.pkl
│
├── Dockerfile
├── Dockerfile.frontend
├── docker-compose.yml
├── requirements.txt
├── .dockerignore
├── .gitignore
└── README.md
```

---

# 🐳 Docker Images

## FastAPI Backend

```
docker pull hitesh2210/student_health_predictor_api
```

Docker Hub:

https://hub.docker.com/r/hitesh2210/student_health_predictor_api

---

## Streamlit Frontend

```
docker pull hitesh2210/student_health_predictor_frontend
```

Docker Hub:

https://hub.docker.com/r/hitesh2210/student_health_predictor_frontend

---

# ▶️ Running the Application

## Clone the repository

```bash
git clone https://github.com/hitesh-2212/STUDENT_HEALTH_DOCKER.git

cd STUDENT_HEALTH_DOCKER
```

## Build the Docker images

### FastAPI

```bash
docker build -t student_health_predictor_api .
```

### Streamlit

```bash
docker build -f Dockerfile.frontend -t student_health_predictor_frontend .
```

---

## Run the containers

### FastAPI

```bash
docker run -d -p 8000:8000 student_health_predictor_api
```

### Streamlit

```bash
docker run -d -p 8501:8501 student_health_predictor_frontend
```

---

# 🌐 Application URLs

FastAPI Swagger UI

```
http://localhost:8000/docs
```

Streamlit

```
http://localhost:8501
```

---

# ☁️ Cloud Deployment

This project is designed to be deployed on AWS EC2 using Docker.

Deployment steps include:

- Launch an EC2 instance
- Install Docker
- Pull Docker images from Docker Hub
- Run the FastAPI and Streamlit containers
- Access the application via the EC2 public IP

---

# 📚 Machine Learning Project

The complete machine learning pipeline, including data preprocessing, model training, evaluation, and notebook implementation, is available in the following repository:

👉 https://github.com/hitesh-2212/student-health-risk-prediction

---

# 🛠️ Tech Stack

- Python
- FastAPI
- Streamlit
- CatBoost
- Scikit-learn
- Pandas
- Docker
- Docker Hub
- AWS EC2 (Deployment Ready)


---

# 👨‍💻 Author

**Hitesh Sirswa**

GitHub:
https://github.com/hitesh-2212

LinkedIn:
https://www.linkedin.com/in/hitesh-sirswa/

---

⭐ If you found this project helpful, please consider giving it a star.

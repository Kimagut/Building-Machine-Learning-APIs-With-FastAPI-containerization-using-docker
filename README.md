# Building-Machine-Learning-APIs-With-FastAPI-containerization-using-docker
Building Machine Learning APIs With FastAPI &amp; containerization using docker
This project provides a complete environment for predicting the likelihood of sepsis in ICU patients using machine learning models. It includes a FastAPI backend for model predictions and a Streamlit frontend for user interaction, all orchestrated with Docker Compose.

# Table of Contents
### Overview
### Features
### Project Structure
### Getting Started
### Prerequisites
### Setup Instructions
### Usage
### Endpoints
### Technologies Used
### Contributing
### License
# Overview
The goal of this project is to identify ICU patients at risk of developing sepsis using machine learning models. It includes:
- A FastAPI backend for serving predictions.
- A Streamlit frontend for user interaction.
- Redis caching for optimizing performance.
# Features
- Model Selection: Choose between XGBoost and Random Forest models.
- API Endpoints: Predict sepsis risk via API.
- User Interface: Input patient data and receive predictions through a web interface.
- Caching: Redis caching to improve performance.
# Project Structure
- Dockerfile-api
- Dockerfile-streamlit
  docker-compose.yml
  requirements_docker_api.txt
  requirements_docker_streamlit.txt
- src
   api
      api.py
      config.py
      .env
  streamlit
    predict.py

# Prerequisites
- Docker
- Docker Compose

# Usage
- Access the FastAPI documentation:
  Navigate to http://localhost:9000/docs to explore the API endpoints.

- Use the Streamlit web interface:
  Open your browser and go to http://localhost:8501 to use the web app.

# Endpoints
## FastAPI Endpoints
- Status Check: GET /
  Checks if the API is online.
- XGBoost Prediction: POST /xgboost_prediction
  Predict sepsis risk using the XGBoost model.
  Request Body: JSON containing patient features.
- Random Forest Prediction: POST /random_forest_prediction
  Predict sepsis risk using the Random Forest model.
  Request Body: JSON containing patient features.
# Technologies Used
- FastAPI: Backend framework for building APIs.
- Streamlit: Frontend framework for building web apps.
- Redis: In-memory data structure store for caching.
- Docker: Containerization platform.
- Docker Compose: Tool for defining and running multi-container Docker applications.


# License
This project is licensed under the MIT License. See the LICENSE file for details.


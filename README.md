# Medvora

A Machine Learning-powered web application using FastAPI and Streamlit to predict heart disease risk based on clinical patient data.

# ⚕️ Medvora.ML

A Machine Learning-powered web application that predicts a patient's risk of heart disease based on clinical data. The project features a RESTful API backend built with **FastAPI** and an interactive, user-friendly frontend built with **Streamlit**.

## 🚀 Features
- **Heart Disease Risk Prediction**: Uses an ML model to evaluate health metrics and predict disease likelihood.
- **FastAPI Backend**: Robust, high-performance API endpoint to serve the prediction model.
- **Streamlit Frontend**: Simple, clean web interface for medical personnel to input patient clinical data.
- **Jupyter Notebooks**: Complete data exploration, preprocessing, and model training pipeline.

## 📂 Project Structure
```text
Medvora/
├── backend/          # FastAPI application & model prediction logic
├── dataset/          # Heart disease dataset (heart.csv)
├── frontend/         # Streamlit web application
├── model_dir/        # Saved/serialized ML models (.joblib)
├── notebook_files/   # Jupyter notebooks for data analysis & training
├── env_template.txt  # Template for environment variables
├── requirements.txt  # Python package dependencies
└── README.md         # Project documentation

## 🛠️ Tech Stack
Backend: FastAPI, Uvicorn, Pydantic
Frontend: Streamlit, Requests
Machine Learning: Scikit-Learn, Pandas, Joblib
Language: Python 3.x

## 💻 Local Setup & Installation
1. Clone the repository
git clone "link_of_this_repo"
cd Medvora

2. Set up a virtual environment
python -m venv .venv
# On Windows
.venv\Scripts\activate
# On Linux/macOS
source .venv/bin/activate

3. Install dependencies
pip install -r requirements.txt

4. Set environment variables
Rename env_template.txt to .env (inside the frontend folder or root, depending on your setup) and define the API_URL:

API_URL=http://localhost:8000/predict-heart-disease

## 🏃‍♂️ Running the Services

# ター Start the Backend (FastAPI)

Open a terminal and run:
uvicorn backend.main:app --reload

# 🌐 Start the Frontend (Streamlit)

Open a second terminal, activate the environment, and run:
streamlit run frontend/app.py

## 🏥 How to Use

1. Open the Streamlit web interface in your browser.
2. Enter the patient's clinical metrics (Age, Sex, Cholesterol, Resting BP, etc.).
3. Click on the 🔍 Predict button.
4. The frontend will communicate with the FastAPI backend and return the prediction (Heart Disease Detected / No Heart Disease Detected).


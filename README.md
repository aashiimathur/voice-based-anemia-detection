# Anemia Detection Using Voice

## Overview

This project is an AI-based system that predicts hemoglobin levels and detects anemia severity using voice recordings. The system analyzes acoustic voice biomarkers such as jitter, shimmer, HNR, and MFCC features to identify voice instability patterns associated with anemia.

The project combines machine learning, speech processing, and a full-stack web application for real-time prediction.

---

# Features

- Upload audio files
- Record voice directly from browser
- Hemoglobin (Hb) prediction
- Anemia severity classification
- Biomarker analysis
- Risk score generation
- Human-readable explanations

---

# Voice Biomarkers Used

- **Jitter** → Frequency instability
- **Shimmer** → Amplitude instability
- **HNR** → Voice clarity/noise level
- **MFCCs** → Spectral speech features

---

# Machine Learning Models Used

The following models were tested:

- Random Forest Regressor
- Gradient Boosting Regressor
- Hist Gradient Boosting Regressor
- Extra Trees Regressor
- SVR
- KNN

### Final Selected Model:
ExtraTreesRegressor

---

# Results

- Regression Accuracy: ~94%
- Classification Accuracy: ~90%
- Classes:
  - Normal
  - Mild
  - Moderate
  - Severe

---

# Tech Stack

## Frontend
- React.js
- CSS

## Backend
- FastAPI
- Python

## Machine Learning & Audio
- Scikit-learn
- Librosa
- Parselmouth
- NumPy
- Pandas

---

# Datasets Used

- VOICED Dataset
- Saarbruecken Voice Database (SVD)

---

# Project Structure

```text
anemia-detection/
│
├── anemia-backend/
│   ├── main.py
│   ├── anemia_classifier.pkl
│   ├── hb_model.pkl
│   └── label_encoder.pkl
│
├── anemia-frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
└── README.md
```

---

# How to Run the Project

## Backend

```bash
cd anemia-backend
pip install -r requirements.txt
uvicorn main:app --reload
```

---

## Frontend

```bash
cd anemia-frontend
npm install
npm start
```

---

# Application Features

- Upload audio in multiple formats
- Record voice directly from browser
- Predict hemoglobin levels
- Detect anemia severity
- Show confidence score
- Generate biomarker analysis

---

# Disclaimer

This project is intended for research and educational purposes only and is not a clinically approved medical diagnostic system.


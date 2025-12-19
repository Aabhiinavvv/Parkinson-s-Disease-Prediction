# 🧠 Parkinson’s Disease Prediction API

A Machine Learning–powered FastAPI application that predicts whether a person has Parkinson’s Disease based on biomedical voice measurements.

---

## 🚀 Features
- Trained ML model using Scikit-learn
- REST API built with FastAPI
- Input validation using Pydantic
- Tested using Swagger UI and Python client
- Ready for deployment

---

## 🧪 Model Inputs
The model uses 22 biomedical voice features such as:
- Fundamental frequency (Fo, Fhi, Flo)
- Jitter & Shimmer metrics
- Noise-to-Harmonics Ratio (NHR)
- Nonlinear dynamical features (RPDE, DFA)
- Spread and PPE values

---

## 📡 API Endpoint

### POST `/parkinson_prediction`

#### Sample Request
```json
{
  "MDVP_Fo_Hz": 119.992,
  "MDVP_Fhi_Hz": 157.302,
  "MDVP_Flo_Hz": 74.997,
  "MDVP_Jitter_percent": 0.00784,
  "MDVP_Jitter_Abs": 0.00007,
  "MDVP_RAP": 0.00370,
  "MDVP_PPQ": 0.00554,
  "Jitter_DDP": 0.01109,
  "MDVP_Shimmer": 0.04374,
  "MDVP_Shimmer_dB": 0.426,
  "Shimmer_APQ3": 0.02182,
  "Shimmer_APQ5": 0.03130,
  "MDVP_APQ": 0.02971,
  "Shimmer_DDA": 0.06545,
  "NHR": 0.02211,
  "HNR": 21.033,
  "RPDE": 0.414783,
  "DFA": 0.815285,
  "spread1": -4.813031,
  "spread2": 0.266482,
  "D2": 2.301442,
  "PPE": 0.284654
}

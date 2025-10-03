# 🌌 AEXIS – Exoplanet Classifier

## 📖 Project Description
AEXIS is a machine learning project designed to classify **exoplanets** based on data from **NASA’s Kepler mission**.  
The model predicts whether an observed candidate is:

- **CONFIRMED** → Verified exoplanet  
- **CANDIDATE** → Potential exoplanet, requires further validation  
- **FALSE POSITIVE** → Incorrect detection

---

## ⚙️ Models
Two models were developed for different purposes:

1. **Full Model (Large, Research-Oriented)**  
   - Trained on ~66 features  
   - High accuracy (~90%)  
   - Used for research, benchmarking, and reporting  

2. **Frontend Model (Lightweight, Production-Ready)**  
   - Trained on **5 selected features**:  
     - `koi_period` (orbital period in days)  
     - `koi_prad` (planet radius in Earth radii)  
     - `koi_smass` (stellar mass in solar masses)  
     - `koi_teq` (equilibrium temperature in Kelvin)  
     - `koi_depth` (transit depth in ppm)  
   - Smaller, faster model optimized for web frontend integration  
   - Accuracy ~69%, with balanced class performance  

---

## 📊 Performance (Summary)

### Full Model
- **Accuracy:** ~90%  
- **Balanced across classes** (especially strong for CONFIRMED & FALSE POSITIVE)  

### Frontend Model
- **Accuracy:** ~69%  
- Good trade-off between speed and interpretability for real-time usage  

---


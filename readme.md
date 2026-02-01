# 🔥 AI-Based Forest Fire & Smoke Detection

## 📌 Project Overview
Forest fires pose a serious threat to ecosystems, wildlife, and human life.  
This project presents an **end-to-end machine learning system** to detect **forest fire and smoke regions** using features extracted from aerial imagery.

The model predicts **fire risk probabilities** for image tiles and converts them into **spatial heatmaps**, enabling **drone-based disaster monitoring and early response**.


## 🎯 Objectives
- Analyze aerial image-derived features for fire and smoke detection
- Train a robust machine learning classifier
- Achieve high accuracy and reliability for disaster scenarios
- Generate spatial fire-risk heatmaps for actionable insights
- Propose a drone-based monitoring strategy


## 📂 Project Structure
Capstone IITH/
│
├── capstone.ipynb # Complete implementation notebook
├── fire_smoke_dataset.csv # Dataset (feature-based)
└── README.md # Project documentation


## 📊 Dataset Description
- Each row represents a **spatial tile** extracted from aerial imagery
- Features include:
  - Spectral features (mean RGB values)
  - Intensity variation
  - Texture and edge information
  - Smoke and haze indicators
  - Thermal indicators (hot pixel fraction)

### 🎯 Target Variable
- `fire_label`
  - `0` → No fire or smoke
  - `1` → Fire or smoke present

## 🧠 Methodology

### 1️⃣ Exploratory Data Analysis (EDA)
- Dataset inspection and cleaning
- Feature distribution analysis
- Class imbalance analysis
- Correlation heatmap visualization

### 2️⃣ Machine Learning Model
- Algorithm: **Random Forest Classifier**
- Reasons for selection:
  - Handles non-linear relationships
  - Robust to noise and outliers
  - Well-suited for tabular feature data
  - Effective with moderately imbalanced datasets

### 3️⃣ Model Evaluation
The model was evaluated using:
- Precision
- Recall
- F1-score
- ROC-AUC

📈 **Achieved ROC-AUC Score:** **0.97**

This indicates excellent discriminative capability between fire/smoke and non-fire regions.

## 🌍 Spatial Risk Analysis
- The trained model generates **fire risk probabilities** for each image tile
- Risk scores range from `0` (safe) to `1` (high risk)
- Simulated spatial coordinates are used to visualize:
  - High-risk clusters
  - Safe regions
- Results are displayed using a **fire-risk heatmap**

## 🚁 Drone-Based Disaster Response Strategy
- High-risk clusters are prioritized for immediate drone surveillance
- Continuous monitoring in critical zones
- Periodic scanning in moderate-risk regions
- Efficient allocation of limited drone resources

This approach bridges **machine learning predictions** with **real-world disaster management**.

## ⚠️ Limitations
- Dataset uses pre-extracted features instead of raw images
- Spatial coordinates are simulated, not real GPS locations
- No temporal modeling of fire spread
- Weather factors (wind, humidity, temperature) not included

## 🔮 Future Improvements
- Use CNNs on raw satellite/drone imagery
- Integrate real geospatial coordinates
- Add temporal modeling for fire spread prediction
- Combine weather data for enhanced accuracy
- Deploy as a real-time monitoring system

## 🏁 Conclusion
This project demonstrates how machine learning can be effectively applied to **early forest fire detection**.  
With a **ROC-AUC score of 0.97**, the model shows strong performance, and the spatial heatmap provides actionable insights for disaster response systems.

The project highlights the potential of AI-driven solutions in environmental protection and emergency management.


## 👩‍💻 Author
**Sowmya Kanithi**

Machine Learning Enthusiast | AI & Data Science Aspirant

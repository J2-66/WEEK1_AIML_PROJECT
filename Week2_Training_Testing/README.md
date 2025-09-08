## 🌊 Water Quality & Pollution Level Classification using Machine Learning

## 📌 Project Overview
This project focuses on **environmental monitoring** by classifying **water quality data** into different **pollution levels** using machine learning.  
The dataset contains water quality parameters like pH, Turbidity, Dissolved Oxygen, Nitrate, Conductivity, and more, collected over time across different locations.

By applying **classification models (Logistic Regression, Random Forest, XGBoost)**, we aim to predict whether a water sample falls into a **safe or polluted category**.  
This helps in early detection of pollution and supports environmental sustainability.

---

## 📊 Dataset
- **Source**: Synthetic *Water Quality and Pollution Monitoring Dataset* (Kaggle)
  
- **Features**:
  
  - **Physico-chemical parameters**: `pH`, `Turbidity`, `DO`, `Nitrate`, `Conductivity`, etc.
    
  - **Temporal data**: `Timestamp` (converted into `year, month, day, hour`)
    
  - **Location**: Encoded into dummy variables
    
- **Target**: `Pollution Level` (categorical classification)

---

## ⚙️ Preprocessing Steps

1. Converted **Timestamp** → datetime & extracted time features (`year, month, day, hour`).
   
2. Dropped original **Timestamp** column (non-numeric).
   
3. One-hot encoded **Location** column.
  
4. Applied **Standard Scaling** for numerical features.  

---

## 🤖 Machine Learning Pipeline

We implemented three ML models for classification:

- **Logistic Regression**
  
- **Random Forest Classifier**
  
- **XGBoost Classifier**

### 📌 Key Results

- **Random Forest & XGBoost** outperformed Logistic Regression.
  
- Cross-validation ensured models generalize well.
  
- Feature Importance plots highlighted which parameters (like **Dissolved Oxygen, pH, Conductivity**) have the strongest impact on pollution level.

---

## 📈 Visualizations

- Correlation heatmap of water quality parameters
  
- Confusion Matrices for each model
  
- Model Accuracy Comparison (bar chart)
  
- Feature Importance (Random Forest & XGBoost)  

---

## 🚀 How to Run
1. Clone the repository:
   
   ```bash
   git clone https://github.com/yourusername/water-quality-classification.git
   
   cd water-quality-classification


2. Install dependencies:
   ```bash
   pip install -r requirements.txt


3. Run preprocessing & ML pipeline:
   ```bash
   python water_quality_classification.py

# 🔮 Future Scope
•	Implement Water Quality Index (WQI) calculation before classification.

•	Deploy as a real-time monitoring dashboard using Streamlit/Flask.

•	Extend dataset with IoT sensor readings for live pollution detection.

•	Use Deep Learning (LSTMs) for time-series pollution forecasting.

# 🙌 Acknowledgements
•	Dataset inspired from Kaggle: Water Quality and Pollution Monitoring Dataset

•	Libraries used: pandas, scikit-learn, xgboost, matplotlib, seaborn

# 👨‍💻 Author
Developed as part of my internship project on Environmental Monitoring using Machine Learning.






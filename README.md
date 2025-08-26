# Absorption Coefficient Prediction using Machine Learning and Neural Networks for Janus Al₂SO monolayer

This repository presents a machine learning approach to predict stress responses under different strain conditions. Seven distinct strain levels (−6%, −4%, −2%, 0%, 2%, 4%, 6%) were simulated, generating a dataset of **14,000 samples**. Multiple regression models were trained and benchmarked to evaluate predictive performance, combining both classical ML methods and deep learning.

It can be easily run in Colab.

---

## Repository Structure
├── dataset/ # Contains the generated dataset from DFT simulation
├── code/ # Python scripts and notebooks for model training and evaluation
└── README.md # Project documentation

---

## Dataset

- **Strain conditions:** −6%, −4%, −2%, 0%, 2%, 4%, 6%  
- **Samples per condition:** 2000  
- **Total dataset size:** 14,000 entries  
- **Preprocessing:**  
  - Normalization applied to inputs and outputs  
  - Dataset split into 80% training and 20% testing  

---

## Models Implemented

The following regression models were trained and evaluated:  

1. Linear Regression  
2. Random Forest Regressor  
3. Support Vector Regressor (SVR)  
4. K-Nearest Neighbors (KNN) Regressor  
5. XGBoost Regressor  
6. LightGBM Regressor  
7. Feedforward Neural Network (NN)  

---

## Evaluation Metrics

Each model was evaluated on the testing set using:  
- **Mean Squared Error (MSE)**  
- **Mean Absolute Error (MAE)**  
- **Coefficient of Determination (R² Score)**  

---

## Results

**Performance comparison of regression models**

| SL No. | Model Name       | MSE    | MAE    | R²    |
|--------|------------------|--------|--------|-------|
| 01     | LinearRegression | 0.2522 | 0.3616 | 0.7489 |
| 02     | RandomForest     | 0.0038 | 0.0261 | 0.9962 |
| 03     | SVR              | 0.0032 | 0.0469 | 0.9969 |
| 04     | KNN              | 0.0076 | 0.0238 | 0.9925 |
| 05     | XGBoost          | 0.0010 | 0.0147 | 0.9990 |
| 06     | LightGBM         | 0.0009 | 0.0140 | 0.9991 |
| 07     | Neural Network   | 0.0001 | 0.0060 | 0.9999 |

---

## Installation & Usage

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/DFT_ML.git
   cd DFT_ML


# 🔎 Exploratory Data Analysis and Regression Models Comparison

## 📌 Project Overview
This project investigates a dataset of musical tracks with various audio features in order to predict **track popularity**.  
The workflow includes:
- Exploratory Data Analysis (EDA),  
- Building and comparing three regression models:  
    1. **Lasso Regression**  
    2. **Random Forest Regression (RFR)**  
    3. **Artificial Neural Networks (ANN / MLP)**
- Comparison of statistical metrics values and error values  

The analysis was carried out in a **Google Colab notebook**.

---

## 🎵 Dataset
The dataset consists of **3,614 tracks** with the following features (after preprocessing):
- `acousticness`,
- `danceability`,
- `duration_ms`,
- `energy`,  
- `instrumentalness`,
- `liveness`,
- `speechiness`,
- `tempo`,
- `valence`,  
- `popularity` (target variable).  

Some categorical fields (`streaming_platform`, `key`, `mode`) and `loudness` were excluded during data preparation because of being NaN and also to simplify the modeling task.  

---

## 🔬 Methodology

### 1. Exploratory Data Analysis (EDA)
- Basic statistics and data structure inspection,  
- Distribution plots for numerical variables,  
- Correlation analysis to identify relationships with **popularity**,  
- Visualizations such as histograms, scatter plots, and heatmaps.  

### 2. Regression Models

- **Artificial Neural Networks (ANN)**  
  Implemented as a Multilayer Perceptron (MLP) with dense layers, trained to approximate complex nonlinear patterns.
  
- **Lasso Regression**  
  Linear regression with L1 regularization, used to shrink less important coefficients and reduce overfitting.  

- **Random Forest Regression (RFR)**  
  An ensemble model based on decision trees. Provides robustness and the ability to capture nonlinear relationships.  

### 3. Evaluation
Models were assessed using multiple error metrics:
- **MAE** (Mean Absolute Error)  
- **MSE** (Mean Squared Error)   
- **R²** (Coefficient of Determination)  

---

## 📊 Results
- All three models were able to capture general trends in the data, but with varying degrees of accuracy.  
- **Random Forest Regression** performed better than Lasso Regression, especially in handling nonlinear dependencies.  
- **Artificial Neural Networks** provided competitive results, but required careful tuning of hyperparameters and longer training time.  
- The comparison highlights the trade-off between interpretability (Lasso), robustness (Random Forest), and flexibility (ANN).  

---

## 🚀 How to Run
This project was developed in **Google Colab**. To reproduce:
1. Open the notebook (.ipynb file) in Colab.  
2. Upload the dataset (`dane_3.csv`).  
3. Run all cells step by step.  

---

## 📌 Summary
The analysis shows that **ensemble and neural methods** outperform simple linear approaches when predicting music popularity.  
While **Lasso Regression** provides interpretability and feature selection, **Random Forest Regression** proved the most reliable on this dataset, and **ANN** showed potential for further improvement with proper optimization.  

---

## 📄 License
This project is released under the MIT License.  

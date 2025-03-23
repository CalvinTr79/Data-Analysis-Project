# Portfolio: Analysis of Bike Rental Data in Seoul 🚲

## 1. Project Overview 📽️  
This project analyzes a public dataset of bike rental demand in Seoul, South Korea. The objective is to examine factors influencing the number of bikes rented daily and apply machine learning models to predict and classify demand levels.

**Key components of the analysis include:**
- Correlation analysis to identify impactful features  
- Regression models (Linear and Polynomial) to assess relationships  
- K-Means clustering to segment demand levels  
- Neural network modeling for improved prediction performance  

---

## 2. Data Source 💽  
The dataset includes daily bike rental figures along with weather and temporal features.

**Important columns:**
- `Rented Bike Count`: Daily rental count (target variable)  
- `Temperature`, `Humidity`, `Wind Speed`, `Rainfall`, etc.  
- Categorical fields: `Seasons`, `Holiday`, `Functioning Day`  

---

## 3. Models Applied  

### 📈 Correlation Analysis  
A heatmap identified **temperature** as having the strongest positive correlation with rentals.

### 🔹 Linear Regression  
Used to model `Temperature` vs. `Rented Bike Count`. Low R² score (−0.04) indicated poor fit.

### 🔹 Polynomial Regression  
Polynomial models (degrees 1–3) showed that:  
- Degree 1 had the best performance (R² = 0.80)  
- Higher degrees led to overfitting  

### 📊 Neural Network  
Implemented a basic neural network model, achieving **R² = 0.877**, the best result in this project.

### 🏘️ K-Means Clustering  
Segmented the data into three demand groups: **Low**, **Average**, and **High** rental days.

---

## 4. Visualizations 🎨  
The project includes:
- Heatmap of feature correlations  
- Regression plots with trendlines  
- Bar charts comparing R² scores  
- Scatter plots of demand clusters  

---

## 5. Repository Structure 📂  
```
📄 Portfolio.ipynb             # Jupyter Notebook with full analysis  
📄 Seoul Bike Data.csv         # Dataset used  
📄 ancient_korea-max.jpg       # Visual element (optional)  
📄 README.md                   # Project overview and documentation  
```

---

## 6. How to Run the Code 🏃  
1. Clone the repo:
```bash
git clone https://github.com/CalvinTr79/Data-Analysis-Project.git
```

2. (Optional) Install dependencies:
```bash
pip install -r requirements.txt
```

3. Launch the notebook:
```bash
jupyter notebook "Portfolio.ipynb"
```

---

## 7. Conclusion 🎬  
This project highlights temperature as a key factor in predicting bike rentals. Polynomial regression and neural networks outperformed other models, while clustering enabled effective segmentation of demand types.

---

## 8. Future Work 🚀  
- Improve outlier detection and handling  
- Integrate external data sources (e.g. public holidays, traffic)  
- Experiment with deeper neural networks or ensemble methods  

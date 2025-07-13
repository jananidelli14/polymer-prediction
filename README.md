# 🧪 Polymer Property Prediction (NeurIPS 2025 Challenge)

This project focuses on predicting key polymer properties such as:

- 🔥 Glass Transition Temperature (Tg)  
- 🧊 Fractional Free Volume (FFV)  
- 🌡️ Thermal Conductivity (Tc)  
- ⚖️ Density  
- 📐 Radius of Gyration (Rg)

using SMILES-based molecular descriptors and machine learning.

## 📁 Dataset
Official dataset provided by [NeurIPS 2025 Open Polymer Prediction Challenge](https://www.kaggle.com/competitions/neurips-open-polymer-prediction-2025).  
Contains:
- `train.csv`
- `test.csv`
- SMILES strings with missing target values

## ⚙️ Methodology
- 📦 Feature extraction using RDKit (MolWt, TPSA, LogP, Rings, etc.)
- 🔍 Data exploration and missing value visualizations
- 🔁 Random Forest Regressor for multi-target prediction
- 📉 Residual analysis and prediction uncertainty estimation
- 📊 PCA, correlation heatmaps, box plots, and feature importance visualizations

## 📊 Visualizations
- Missing value maps (static + interactive)
- Correlation matrices
- PCA plots (colored by FFV)
- Feature importance heatmaps
- SMILES length analysis
- Prediction vs Actual and Uncertainty vs Error plots

## 🧠 Model
- ✅ Random Forest Regressor
- 📈 MAE evaluated for each target
- 🧪 Submission generated for test set

## 🛠️ Requirements
Install key dependencies:
```bash
pip install rdkit-pypi scikit-learn seaborn matplotlib pandas numpy plotly

# Climatewins_Machine_Learning_Project

## Project Context
This project is part of the CareerFoundry Data Analytics program.  
I assumed the role of a data analyst for **Climatewins**, a (fictional) European nonprofit dedicated to using machine learning to anticipate the consequences of climate change.  

## Overview
The project demonstrates a progression from classical machine learning on structured weather data to deep learning with imagery, and explores future-facing proposals for climate modeling:

- Weather classification with historical observations  
- Image classification using Convolutional Neural Networks (CNNs)  
- Proposals for radar/satellite imagery analysis, climate twin city identification, and hybrid models with IPCC projections  

## Data
- **Source**: European Climate Assessment & Dataset Project (ECA&D)  
- **Coverage**: Daily observations from 18 weather stations (1960–2022) across mainland Europe  
- **Variables**: 9 weather features, including temperature, precipitation, and cloud cover  

## Languages & Libraries
- **Python**  
- **Core Libraries**:  
  - Data Handling & Analysis: `pandas`, `numpy`  
  - Visualization: `matplotlib`, `seaborn`, `plotly`  
  - Machine Learning (classical): `scikit-learn` (KNN, Decision Trees, Random Forest, ANN, PCA, Clustering)  
  - Deep Learning: `tensorflow` / `keras` (CNN, RNN, EfficientNetB0 for transfer learning)  

## 1. Weather Classification 
- **Task**: Classify daily weather as pleasant or unpleasant  
- **Challenge**: Class imbalance (fewer pleasant days)  
- **Evaluation Metric**: Weighted F1 score (more reliable than accuracy)  
- **Models Tested**:  
  - K-Nearest Neighbors (KNN)  
  - Decision Tree  
  - Artificial Neural Network (ANN)  
  - Random Forest (optimized, achieved weighted F1 ≈ 0.99)  
- **Key Finding**: Only three features (max temperature, precipitation, sunshine) were sufficient for strong classification → lower computational cost, robust to missing data  

## 2. Deep Learning Models 
- **CNN Models**:  
  - Classified pleasant vs. unpleasant days  
  - Classified weather imagery into categories (*Cloudy, Rain, Shine, Sunrise*)  
- **Best Result**: Transfer learning with **EfficientNetB0 CNN** achieved the highest performance with **Weighted F1 ≈ 0.92**  
- **Proof of Concept**: Demonstrates potential for radar and satellite image classification  

## 3. Future Directions
- **Radar & Satellite Imagery**  
  - CNNs, ConvLSTMs, GANs, and Transformers for storm detection and nowcasting  
- **Climate Twin Cities**  
  - PCA + clustering for identifying climate families across cities  
  - Graph Neural Networks for mapping climate similarity networks  
- **Hybrid Models with IPCC Projections**  
  - Combining historical weather with global climate scenarios to anticipate local risks  

## Why It Matters
Machine learning provides a bridge between climate science and decision-making:  

- **Simple models** → practical, fast, and scalable  
- **Deep models** → unlock new possibilities in imagery and climate adaptation  
- **Together** → data-driven tools for resilience  

## Folders
- **01 Project Management**: Project brief  
- **02 Data**: (Data not uploaded due to size limitations)  
- **03 Scripts**: Python code and Jupyter notebooks  
- **04 Analysis**: Visualizations for exploratory analysis and insights  
- **05 Sent to Client**: Progress report and final project presentations  

# House Price Prediction with SHAP Analysis

This repository contains a project for predicting house prices based on various features using machine learning. It includes exploratory data analysis (EDA), feature engineering, model training, and interpretability analysis with SHAP (SHapley Additive exPlanations) to understand feature contributions.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [References](#references)

## Overview
The aim of this project is to predict house prices using a dataset of property attributes. We use machine learning algorithms to build a predictive model and leverage SHAP to interpret the influence of each feature on the predictions. SHAP values provide a way to break down predictions into the contributions of each feature, helping to understand model decisions.

## Dataset
The dataset used in this project is from [Kaggle](https://www.kaggle.com/datasets), containing information about various properties, including features like:
- Square footage
- Location attributes
- Year built
- Number of bedrooms and bathrooms
- And more...

This data allows us to explore and identify factors influencing house prices and helps build a robust predictive model.

## Project Structure
The repository structure is as follows:
```plaintext
house-price-prediction/
├── data/                   # Folder for storing the dataset
├── notebooks/              # Jupyter notebooks with EDA, modeling, and SHAP analysis
├── src/                    # Python scripts for data processing and model functions
├── README.md               # Project README file
└── requirements.txt        # List of dependencies
```

- **`notebooks`**: Contains Jupyter Notebook files where the project workflow is demonstrated, including data exploration, feature engineering, model training, and SHAP explanations.
- **`src`**: Python modules for reusable functions for data preprocessing, feature engineering, and model evaluation.

## Installation
To set up the project environment, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/Kevser-Yilmaz/house_price_prediction.git
   cd house_price_prediction
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

> **Note**: Ensure that you have Jupyter Notebook installed to run the `.ipynb` files, as well as packages like `pandas`, `scikit-learn`, `shap`, and `matplotlib` for data processing, modeling, and visualization.

## Usage
To run the project, you can start by exploring the Jupyter Notebooks in the `notebooks` directory. These notebooks cover each step of the analysis:

1. **Data Exploration and Preprocessing**: Open `data_exploration.ipynb` to inspect data distributions, correlations, and missing values.
2. **Feature Engineering and Model Training**: Use `model_training.ipynb` to preprocess data, engineer features, and train a predictive model.
3. **Model Interpretation with SHAP**: Run `shap_analysis.ipynb` to see feature contributions using SHAP values, providing insights into model predictions.

## Results
The model achieves good predictive accuracy on the test data. Key findings from the SHAP analysis reveal that certain features have strong impacts on the predictions, such as:
- **Location and Size**: Larger houses in high-demand locations generally have higher prices.
- **Property Age**: Newer properties often correlate with higher prices, though this varies based on location and size.
- **Additional Features**: Attributes like the number of bathrooms, garage size, and renovations significantly influence the price.

The SHAP visualizations (summary plots, dependence plots) provide a clearer understanding of these effects, helping to interpret model behavior.

## References
- [Kaggle Dataset](https://www.kaggle.com/datasets)
- Lundberg, S. M., & Lee, S. I. (2017). A Unified Approach to Interpreting Model Predictions. *Advances in Neural Information Processing Systems, 30*, 4765-4774.
  
Feel free to explore the code and modify it for your own needs. Contributions and improvements are welcome!

---

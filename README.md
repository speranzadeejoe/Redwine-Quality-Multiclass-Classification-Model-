# Redwine-Quality-Multiclass-Classification-Model-
# Redwine Quality Multiclass Classification Model

## Overview
This project aims to develop a **Deep Learning Multiclass Classification Model** to predict the quality of red wine based on its physicochemical properties. The dataset used for this project is the **Red Wine Quality Dataset**, sourced from the UCI Machine Learning Repository.

## Dataset
The dataset contains **1599 samples** of red wine, each described by **11 physicochemical properties**, including:
- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol

The target variable is **wine quality**, rated on a scale from 3 to 8.

## Objective
The goal is to build a **deep learning model** that classifies wine quality into different categories (multiclass classification). The architecture implemented is a **Neural Network (ANN)** with multiple hidden layers.

## Preprocessing Steps
1. **Handling Missing Values**: Checked and confirmed that the dataset has no missing values.
2. **Feature Scaling**: Standardized features using **MinMaxScaler**.
3. **Data Splitting**: Divided into **training (80%)** and **testing (20%)** sets.
4. **Class Balancing**: Applied **SMOTE (Synthetic Minority Over-sampling Technique)** to address class imbalance.

## Model Architecture
- **Input Layer**: 11 neurons (one for each feature)
- **Hidden Layers**: Multiple dense layers with ReLU activation
- **Output Layer**: Softmax activation function for multiclass classification
- **Loss Function**: Categorical Cross-Entropy
- **Optimizer**: Adam
- **Metrics**: Precision, Accuracy

## Model Performance Metrics
Each model was evaluated using:
- **Accuracy**
- 
## Installation & Dependencies
To run this project, install the following dependencies:
```bash
pip install numpy pandas scikit-learn tensorflow keras seaborn matplotlib imbalanced-learn
```

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Redwine-Quality-Multiclass-Classification-Model.git
   cd Redwine-Quality-Multiclass-Classification-Model
   ```
2. Run the model script:
   ```bash
   python model_training.py
   ```

## Results & Analysis
- The **SHAP (SHapley Additive exPlanations)** method was used to interpret model predictions.
- **Feature Importance Analysis** revealed that **alcohol, volatile acidity, and sulphates** were the most influential factors in determining wine quality.

## Future Work
- Implement **hyperparameter tuning** for better performance.
- Deploy the model using **Flask or FastAPI**.
- Expand the dataset for improved generalization.

## Contributors
- **Speranza Deejoe**

## License
This project is licensed under the **MIT License**.

# Customer Churn Prediction using Neural Networks

**Project Overview**
This project aims to predict customer churn in a banking dataset using a Neural Network (NN). Churn is defined as customers who exited the bank (target: Exited = 1). We use deep learning to model this binary classification problem and evaluate its performance using various metrics.

**Dataset Summary**
- Target Variable: Exited (0 = Stayed, 1 = Left)
- Features: 9 numerical/categorical features (after preprocessing)
- Size: 10,000 records
- Split: 80% Training (8,000), 20% Testing (2,000)

**Project Steps**
**1. Exploratory Data Analysis (EDA)**
- Handled missing values and outliers
- Performed univariate and bivariate analysis
- Verified class imbalance

**2. Data Preprocessing**

- Feature and target separation: X and y
- Train-test split (80-20)
- Feature scaling with StandardScaler
  
**3.  Neural Network Model**
   
   Architecture:

- **Input Layer** : Accepts 9 features (after preprocessing and encoding)              
- **Dense(10)**   : First hidden layer with 10 neurons, `ReLU` activation              
- **Dense(20)**   : Second hidden layer with 20 neurons, `ReLU` activation             
- **Dense(10)**   : Third hidden layer with 10 neurons, `ReLU` activation              
- **Dense(1)**    : Output layer with 1 neuron, `Sigmoid` activation for binary output 

Compilation & Training
- Loss Function: Binary Cross-Entropy
- Optimizer: Adam
- Epochs: 50
- Validation Split: 20% of training data


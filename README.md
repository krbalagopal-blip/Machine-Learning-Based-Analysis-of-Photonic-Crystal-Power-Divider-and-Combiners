# Machine-Learning-Based-Analysis-of-Photonic-Crystal-Power-Divider-and-Combiners
## Overview

This repository contains the implementation of Machine Learning models for predicting the output power distribution of **Photonic Crystal Wilkinson Power Dividers and Power Combiners**. The project combines **Photonics** and **Machine Learning** to accurately predict power distribution using the **scattering rod radius (r2)** as the input parameter.

The datasets used in this project are generated from photonic crystal simulations, and multiple regression algorithms are implemented to compare prediction performance.

The repository includes implementations for:

- 2-Port Wilkinson Power Divider
- 2-Port Wilkinson Power Combiner
- 4-Port Wilkinson Power Divider
- 4-Port Wilkinson Power Combiner

---

## Repository Structure

```
.
├── 2 port divider.py
├── 2port combiner.py
├── 4 port divider.py
├── 4port combiner.py
│
├── 2port dataset 1000.xlsx
├── 2_port_augmented_dataset_1000.csv
├── 4port_datasetaug_1000.csv
├── 4_Port_Power_Combiner_Augmented_1000.csv
│
├── model/
├── plots/
└── README.md
```

---

# Dataset Mapping

| Python File | Dataset |
|-----------------------|--------------------------------------------|
| 2 port divider.py | 2port dataset 1000.xlsx |
| 2port combiner.py | 2_port_augmented_dataset_1000.csv |
| 4 port divider.py | 4port_datasetaug_1000.csv |
| 4port combiner.py | 4_Port_Power_Combiner_Augmented_1000.csv |

---

# Machine Learning Models

The following Machine Learning algorithms are implemented:

- Random Forest Regression
- AdaBoost Regression
- Support Vector Regression (SVR)
- Linear Regression
- K-Nearest Neighbors (KNN) *(2-Port Divider only)*

---

# Input and Output Parameters

## 2-Port Divider

Dataset:
```
2port dataset 1000.xlsx
```

Input:
```
r2
```

Outputs:
```
port1
port2
```

---

## 2-Port Combiner

Dataset:
```
2_port_augmented_dataset_1000.csv
```

Input:
```
r2
```

Output:
```
Port 1
```

---

## 4-Port Divider

Dataset:
```
4port_datasetaug_1000.csv
```

Input:
```
r2
```

Outputs:
```
port1
port2
port3
port4
```

---

## 4-Port Combiner

Dataset:
```
4_Port_Power_Combiner_Augmented_1000.csv
```

Input:
```
r2
```

Output:
```
Port 1
```

---

# Performance Evaluation

Each model is evaluated using:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score
- Prediction Accuracy

---

# Requirements

- Python 3.10+
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn
- Joblib
- OpenPyXL

Install dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn joblib openpyxl
```

---

# Running the Programs

### 2-Port Divider

```bash
python "2 port divider.py"
```

### 2-Port Combiner

```bash
python "2port combiner.py"
```

### 4-Port Divider

```bash
python "4 port divider.py"
```

### 4-Port Combiner

```bash
python "4port combiner.py"
```

---

# Generated Outputs

The programs generate:

- Trained Machine Learning Models (.pkl)
- Prediction Results
- Predicted vs Actual Comparison
- Performance Metrics
- Training Graphs
- Prediction Plots
- Batch Prediction Results

---

# Applications

- Photonic Crystal Devices
- Silicon Photonics
- Optical Communication Systems
- Integrated Photonic Circuits
- Optical Power Divider Design
- Optical Power Combiner Design
- Artificial Intelligence in Photonics

---

# Future Scope

- Deep Learning Models
- Physics-Informed Neural Networks (PINNs)
- AI-assisted Photonic Circuit Design
- Integration with OptiFDTD and Lumerical
- Real-time FPGA-based Prediction
- Extension to Higher-Port Wilkinson Structures

---

# Author

**K. R. Balagopal**

B.Tech Electronics and Communication Engineering

Research Areas:
- Machine Learning
- Photonics
- Embedded Systems
- Optical Communication
- Artificial Intelligence

---

## License

This project is developed for **academic and research purposes**. You are free to use and modify the code with appropriate citation.

---

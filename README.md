# AI in Cyber

## AI-Driven Cyber Threat Awareness and Detection 

This cybersecurity project that applies **Data Analytics, Machine Learning, and Deep Learning** techniques to network traffic data for identifying **Benign/Normal** and **Reconnaissance OS Scan/Suspicious** traffic.

The project is implemented in **Python using Jupyter Notebook** and follows a complete analytical workflow:

**Data → Inspection → EDA → Preprocessing → Machine Learning → Deep Learning → Model Comparison → Cybersecurity Insights**

---

## 📁 Project Structure

```text
AI in Cyber/
│
├── cyber_threat_detection.ipynb
│
└── README.md
```

### `cyber_threat_detection.ipynb`

The main Jupyter Notebook containing:

* Dataset loading and inspection
* Data quality analysis
* Cybersecurity exploratory data analysis
* Feature preparation
* Logistic Regression
* Decision Tree
* MLP Neural Network
* Confusion matrices
* Classification reports
* Feature importance
* Model performance comparison
* Training-time analysis
* Practical feasibility analysis

---

## 🎯 Project Objective

The main objective of this project is to analyze network traffic and develop classification models that can distinguish between:

* **Benign / Normal traffic**
* **Recon OS Scan / Suspicious traffic**

The project also compares traditional machine-learning approaches with a neural-network-based deep-learning approach.

---

## 🤖 Models Implemented

### 1. Logistic Regression

Used as the **traditional machine-learning baseline**.

### 2. Decision Tree

Used as an **interpretable non-linear classifier** and for analyzing feature importance.

### 3. MLP Neural Network

A **Multi-Layer Perceptron** is used as the deep-learning prototype.

Architecture:

```text
Input Features
      ↓
64 Neurons
      ↓
32 Neurons
      ↓
Output
 ┌────┴────┐
 ▼         ▼
Benign   Suspicious
```

---

## 📊 Model Evaluation

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* Training Time

The final comparison helps determine which approach provides the best balance between **performance, interpretability, computational cost, and practical cybersecurity use**.

---

## 🔐 Cybersecurity Focus

The project focuses on identifying patterns associated with reconnaissance activity in network traffic.

The analysis investigates:

* Destination ports
* Packet behavior
* Flow duration
* Forward and backward traffic
* Active and idle behavior
* Feature correlations
* Important network-flow characteristics

The project is intended as an **academic prototype** and not as a production-ready intrusion detection system.

---

## 🧰 Technologies

* Python
* Jupyter Notebook
* NumPy
* Pandas
* Scikit-learn
* Matplotlib
* Plotly

---

## 📂 Dataset

The project uses two datasets:

1. **Benign Traffic**
2. **Recon OS Scan**

After combining the datasets, the final dataset contains:

* **117,937 records**
* **80 columns**

Target labels:

```text
0 → Benign / Normal
1 → Recon OS Scan / Suspicious
```

The dataset is analyzed for class distribution, data quality, feature behavior, and relationships between network characteristics.

> Dataset files are not included in this repository unless redistribution is permitted by their source/license.

---

## 🔄 Project Workflow

```text
Network Traffic Data
        ↓
Dataset Loading
        ↓
Data Inspection
        ↓
Data Quality Analysis
        ↓
Dataset Combination
        ↓
Cybersecurity EDA
        ↓
Feature Preparation
        ↓
Train/Test Split
        ↓
┌───────────────┬───────────────┬───────────────┐
│               │               │
▼               ▼               ▼
Logistic       Decision         MLP
Regression      Tree         Neural Network
│               │               │
└───────────────┴───────────────┘
                ↓
       Model Evaluation
                ↓
 Accuracy / Precision / Recall / F1
                ↓
       Training Time Analysis
                ↓
       Practical Feasibility
```

---

## 📈 Data Analyst Perspective

The project follows a practical data-analyst workflow:

1. **Understand the data**
2. **Check data quality**
3. **Understand the target variable**
4. **Analyze class distribution**
5. **Explore cybersecurity patterns**
6. **Prepare features**
7. **Build predictive models**
8. **Evaluate model performance**
9. **Compare different approaches**
10. **Generate actionable cybersecurity insights**

This makes the project not only an AI implementation but also a **data-analysis-driven cybersecurity project**.

---

## ⚠️ Data Leakage Prevention

To ensure that models learn from actual network characteristics rather than information that directly reveals the target:

* `Label` is used only as the target.
* `Traffic_Type` is excluded from model features because it identifies the source dataset/class.
* `Dst_Port_Category` is used for EDA but excluded from the baseline ML feature set.

This helps maintain a more meaningful classification setup.

---

## 🚀 How to Run

### 1. Create the environment

```bash
conda create -n cyber_ai python=3.11
```

### 2. Activate it

```bash
conda activate cyber_ai
```

### 3. Install dependencies

```bash
pip install numpy pandas scikit-learn matplotlib plotly jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open

```text
cyber_threat_detection.ipynb
```

Run the notebook cells sequentially.

---

## 📌 Learning Outcomes

This project demonstrates:

* Cybersecurity data analysis
* Exploratory Data Analysis
* Data preprocessing
* Feature analysis
* Data leakage prevention
* Logistic Regression
* Decision Trees
* Neural Networks
* Classification metrics
* Confusion matrices
* Feature importance
* Model comparison
* Training-time analysis
* Practical model selection

---

## 🔮 Future Improvements

Possible future extensions include:

* Random Forest
* Gradient Boosting
* Hyperparameter optimization
* Cross-validation
* Additional attack categories
* Anomaly detection
* SHAP-based explainability
* Real-time network monitoring
* Deployment as a cybersecurity dashboard

---

## ⚠️ Disclaimer

This project is developed for **academic and educational purposes**. The prototype should not be considered a production-ready cybersecurity or intrusion-detection system.

---

## 👩‍💻 Project

**Project Name:** AI in Cyber
**Notebook:** `cyber_threat_detection.ipynb`
**Domain:** Artificial Intelligence + Cybersecurity + Data Analytics
**Implementation:** Python / Jupyter Notebook

# Scientific Heart Disease Fusion - Visual & Computational Analytics

Advanced scientific analytics for the exploration, latent decomposition, and predictive classification of heart disease risk, combining scientific visualization (SciViz) techniques, unsupervised multi-view modeling, and explainable machine learning (XAI).

---

## 📊 Contents

This repository contains:

* **Complete Analysis** (`Scientific_visualization.ipynb`)
Jupyter notebook with the entire data-auditing pipeline, latent decomposition (PCA), clustering (K-Means), predictive modeling (Random Forest), and advanced reliability metrics.

* **Project Presentation** (`Scientific_Visualization_Heart_Project_Draft.pptx`)
Complete discussion slides, structured to map the convergence between visual analysis and computational results.

* **Dataset** (`heart.csv`)
Clinical database containing patient physiological, demographic, and diagnostic profiles.

---

## 🎯 Objectives

### Data Quality Audit

Detect dataset integrity, verify cohort balance, and map linear and distributional feature interactions.

### High-Dimensional Analytics

Visualize patient geometric trajectories in multidimensional space before latent reduction.

### Multi-View Factor Fusion

Simulate advanced data fusion dynamics by separating parameters into two views (Clinical View and Diagnostic View) to extract shared latent factors (MOFA-style approach – Multi-Omics Factor Analysis).

### Unsupervised Strategy

Cluster patient profiles purely geometrically using K-Means, validating cohort homogeneity using Silhouette analysis.

### Computational Validation

Train a Random Forest model to validate the latent space, testing its transparency (*Global Explainability*) and medical reliability (*Probability Calibration Curve*).

---

## 📦 Installation

### Prerequisites

* Python 3.8+
* Google Colab or local Jupyter Notebook

### Environment Setup

#### 1. Clone the repository

```bash
git clone https://github.com/MartinaFilice03/scientific-heart-fusion.git
cd scientific-heart-fusion
```

#### 2. Install dependencies

```bash
pip install pandas numpy seaborn matplotlib scikit-learn scipy
```

#### 3. Verify the environment

```bash
python -c "import pandas, numpy, seaborn, matplotlib, sklearn, scipy; print('Environment successfully configured!')"
```

---

## 🚀 Usage

### Run Complete analysis

Open the notebook via Google Colab or Jupyter Lab:

```bash
jupyter lab Scientific_visualization.ipynb
```

Run the cells sequentially to generate:

* Analytical logs
* Structural audits
* Scientific visualizations
* Predictive results
* Interpretive reports

---

## 📁 Repository Structure

```plaintext
scientific-heart-fusion/
│
├── Scientific_visualization.ipynb # Main Notebook
│
├── scientific_visualization.py # Python script to generate the graphs
│
├── data/
│ └── heart-con-duplicati
│ └── heart-senza-duplicati
│
└── README.md # This file
```

---
## Dataset Description

The dataset used in this project (`heart.csv`) contains clinical and demographic data collected to support the classification and prediction of heart disease risk. The dataset consists of **14 attributes** (columns) described below:

### Feature Overview

| Column | Type | Description | Values / Legend |
| :--- | :--- | :--- | :--- |
| **age** | Numerical | Age of the patient in years. | - |
| **sex** | Binary | Biological sex of the patient. | `1` = Male<br>`0` = Female |
| **cp** | Categorical | Chest pain type experienced by the patient. | `0` = Typical angina<br>`1` = Atypical angina<br>`2` = Non-anginal pain<br>`3` = Asymptomatic |
| **trestbps**| Numerical | Resting blood pressure (in mm Hg on admission to the hospital). | - |
| **chol** | Numerical | Serum cholesterol level in mg/dl. | - |
| **fbs** | Binary | Fasting blood sugar > 120 mg/dl. | `1` = True<br>`0` = False |
| **restecg** | Categorical | Resting electrocardiographic results. | `0` = Normal<br>`1` = ST-T wave abnormality<br>`2` = Showing probable or definite left ventricular hypertrophy |
| **thalach** | Numerical | Maximum heart rate achieved during the stress test. | - |
| **exang** | Binary | Exercise-induced angina. | `1` = Yes<br>`0` = No |
| **oldpeak** | Numerical | ST depression induced by exercise relative to rest. | Continuous decimal value |
| **slope** | Categorical | The slope of the peak exercise ST segment. | `0` = Upsloping<br>`1` = Flat<br>`2` = Downsloping |
| **ca** | Numerical | Number of major vessels (0-3) colored by fluoroscopy. | Integer from `0` to `4` (including potentially missing/null values) |
| **thal** | Categorical | Results of the thalassemia blood test. | `1` = Normal<br>`2` = Fixed defect<br>`3` = Reversable defect |
| **target** | Binary | Target variable (presence or risk of heart disease). | `1` = Presence / Higher risk<br>`0` = Absence / Lower risk |

### Data Note
*The raw data file may contain duplicate records that require a preliminary data cleaning and preprocessing step before being fed into Machine Learning models.*

--

## 🔬 Methodology & Pipeline Chronology

The framework is divided into self-consistent computational phases.

### Phase 0 — Pipeline Initialization, Data Sourcing & Architectural Setup

* Environment Stabilization
* Scientific Libraries Import
* Data Loading
* Matrix Preparation

---

### Phase 1 — Data Quality Audit & Exploratory Expression Profiling

* Dataset Completeness Verification (**0% Missing Values**)
* Target Balance Analysis (**165 Healthy vs. 138 Diseased Patients**)
* Symmetrical Correlation Matrix Construction

---

### Advanced Multi-Panel Violin Framework

Detailed analysis of biomarker skewness using:

* Violin Plot
* Combined Strip Plots

---

### High-Dimensional Geometric Trajectories

Multidimensional pre-scaling trajectories using:

* Andrews Fourier Curves
* Standardized Parallel Coordinates Plot

---

### Latent Space Decomposition & Unsupervised Clustering

Application of:

* PCA
* Scree Plot
* Biplot
* K-Means Clustering
* Silhouette Profile Analysis

---

### Multi-View Integration (Late Fusion Framework)

Separation into:

* Clinical View
* Diagnostic View

Analyses performed:

* Shared Latent Factor Extraction
* Variance Explained per View Matrix
* Feature Loading Profile
* Hierarchical Clustered Heatmap

---

### Predictive Modeling & Operational Auditing

Training and optimization of:

* Random Forest Classifier

Evaluation using:

* Confusion Matrix
* ROC–AUC
* Precision–Recall Curve

---

### Probability Calibration & Reliability Assessment

Validation of probabilistic reliability using:

* Reliability Diagram
* Probability Calibration Curves

---

### Global Explainability (XAI)

Model interpretability through:

* Mean Decrease in Gini Impurity
* Clinical Feature Ranking
* Comparison with Visual Evidence

---

## 📈 Main Results
### Visual-Computational Concordance

The dominant geometric vectors found in the PCA biplot and stratification boxplots coincide with the most influential features selected by the Random Forest model.

### Clinical Reliability

The decision forest achieves an accuracy of **84%**.

The **Reliability Diagram** shows a good match between predicted probabilities and observed disease frequency.

### Multi-View Effectiveness

The decomposition of latent factors allows for more rigorous isolation of high-risk myocardial disease phenotypes compared to healthy profiles.

---

## 🛠️ Technologies Used

### Python 3.8+

### Pandas & NumPy

Hierarchical data auditing and matrix calculations.

### Matplotlib & Seaborn

Advanced scientific visualization.

### Scikit-learn

Supervised and unsupervised machine learning.

### SciPy

Fourier analysis, descriptive statistics, and distribution metrics.

---

## 📄 License

This project was developed for academic and research purposes as part of the Scientific Visualization course.

---

## 👤 Authors

**Martina Filice**
**Corinne D’Elia**

University of Milan
Scientific Visualization Course

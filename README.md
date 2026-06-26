# Scientific Heart Disease Fusion - Visual & Computational Analytics

Advanced scientific analytics for the exploration, latent space decomposition, and predictive classification of heart disease risk. This repository implements a robust data-auditing and scientific visualization (SciViz) pipeline combined with unsupervised multi-view alignment and Explainable AI (XAI) diagnostics.

---

## 📊 Contents

This repository contains:

* **Complete Interactive Analysis** (`Scientific_visualization.ipynb`)
  Jupyter notebook with the entire data-auditing pipeline, outlier detection, latent decomposition (PCA), unsupervised clustering, multi-view late fusion, and global model explainability.

* **Production Script** (`scientific_visualization.py`)
  Python source code compiled to clean the data, execute the mathematical models, and output the advanced scientific visualizations.

* **Raw Dataset** (`data/heart-con-duplicati.xlsx`)
  Clinical database containing original patient physiological, demographic, and diagnostic profiles (including repeated records).

* **Consolidated Dataset** (`data/heart-senza-duplicati.xlsx`)
  Preprocessed clinical database with exact duplicate profiles removed to prevent statistical bias.

---

## 🎯 Project Objectives

### Data Quality Audit & Filtering
Verify dataset integrity through matrix completeness checks, continuous feature outlier screening, exact duplicate cleansing, and multi-scale cross-correlation profiling.

### Latent Space Deconstruction
Reduce the high-dimensional standardized feature space using Principal Component Analysis (PCA) to map structural biplots and analyze individual component explained variance.

### Unsupervised Partitioning Validation
Cluster patient profiles purely geometrically using K-Means and Agglomerative Hierarchical Linkage, cross-verifying cluster boundaries with label-invariant consensus metrics (ARI, NMI).

### Multi-View Late Fusion Framework
Simulate a multi-omics block structure by separating variables into distinct *Clinical/Demographic View* and *Diagnostic/Stress-Test View* to extract and plot cross-domain Euclidean similarities.

### Computational Diagnostics & XAI
Train an Ensemble Random Forest to map global feature importance (Gini Impurity) and fit a multivariable Logistic Regression model to calculate exact adjusted Odds Ratios ($OR$) and $95\%$ Confidence Intervals.

---

## 📦 Installation

### Prerequisites
* Python 3.8+
* Jupyter Lab / Jupyter Notebook or Google Colab environment

### Environment Setup

#### 1. Clone the repository
```bash
git clone [https://github.com/MartinaFilice03/Scientific-heart-fusion.git](https://github.com/MartinaFilice03/Scientific-heart-fusion.git)
cd Scientific-heart-fusion
```

#### 2. Install dependencies

```bash
pip install pandas numpy seaborn matplotlib scikit-learn scipy statsmodels openpyxl
```

#### 3. Verify the environment

```bash
python -c "import pandas, numpy, seaborn, matplotlib, sklearn, scipy, statsmodels; print('Environment successfully configured!')"
```

---

## 🚀 Usage

### Run Complete analysis

Open and run the core interactive notebook:

```bash
jupyter lab Scientific_visualization.ipynb
```

Or execute the production script sequentially to generate the scientific plots:
```bash
python scientific_visualization.py
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
├── Scientific_visualization.ipynb    # Main Analysis Notebook
├── scientific_visualization.py       # Python Production Script
│
├── data/
│   ├── heart-con-duplicati.xlsx      # Raw Dataset (with duplicates)
│   └── heart-senza-duplicati.xlsx    # Clean Dataset (without duplicates)
│
└── README.md                         # Project Documentation
```

---
## Dataset Description

The dataset used in this project (`heart-con-duplicati.xlsx`) contains clinical and demographic data collected to support the classification and prediction of heart disease risk. The dataset consists of **14 attributes** (columns) described below:

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

## 🔬 Methodology & Pipeline Chronology

The framework is divided into self-consistent computational phases:

* **Phase 0 — Pipeline Initialization, Data Sourcing & Architectural Setup:** Stabilization of the computational environment (`Warning Filter`) and loading of scientific dependencies.
* **Phase 1 — Data Quality Audit & Exploratory Expression Profiling:** Verification of matrix completeness and removal of duplicate records to ensure unique patient profiles.
* **Phase 2 - Full Cross-Correlation Matrix:** Analysis of global dataset associations through a full symmetrical cross-correlation matrix.
* **Phase 3 — Data Preprocessing, Feature Scaling & Geometric Alignment:** Target isolation and standard Z-score feature scaling to ensure isotropic variance across features.
* **Phase 4 — Exploratory Data Analysis & Primary Correlation Insights:** Calculation of targeted Pearson correlation coefficients relative to the diagnostic endpoint (`target`).
* **Phase 5 — Latent Space Geometry & Dimensionality Reduction (PCA Biplot):** Dimensionality reduction via PCA, individual/cumulative variance computation (Scree Plot), and loading vectors projection (Biplot).
* **Phase 6 — Latent Space Geometry & 2D Cohort Projections:** Two-dimensional patient space mapping and mathematical optimization of cluster numbers (Elbow Method and Silhouette Score).
* **Phase 7 — Unsupervised Partitioning & Latent Space Boundary Auditing (K-Means Evaluation):** Unsupervised clustering ($K=2$), concordance index calculations (ARI, NMI), and topological validation via Hierarchical Linkage Dendrograms.
* **Phase 8 — Advanced Patient Distribution & Biomarker Stratification:** Evaluation of main biomarker population densities (`age`, `thalach`, `oldpeak`) stratified by clinical cohort.
* **Phase 9 — Multi-Source Data Fusion (Integrating Clinical and Diagnostic Profiles):** Late Fusion of the primary latent components from separate views (*Clinical* vs *Diagnostic*) and calculation of patient Euclidean distance matrices.
* **Phase 10 — Global Model Explainability & Computational Pathology Drivers:** Predictive validation of an ensemble Random Forest (Confusion Matrix, ROC-AUC), feature importance ranking (Gini Impurity), and multivariable Logistic Regression Odds Ratios ($OR$, $95\%$ CI).

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

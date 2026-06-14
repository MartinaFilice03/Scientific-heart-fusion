# Scientific Heart Disease Fusion - Visual & Computational Analytics

Analisi scientifica avanzata per l'esplorazione, la scomposizione latente e la classificazione predittiva del rischio cardiologico, combinando tecniche di visualizzazione scientifica (SciViz), modellazione non supervisionata multi-vista e machine learning spiegabile (XAI).

---

## 📊 Contenuto

Questo repository contiene:

* **Analisi completa** (`Scientific_visualization.ipynb`)
  Notebook Jupyter con l'intera pipeline di data-auditing, scomposizione latente (PCA), clustering (K-Means), modellazione predittiva (Random Forest) e metriche di affidabilità avanzate.

* **Presentazione del Progetto** (`Scientific_Visualization_Heart_Project_Draft.pptx`)
  Slide complete per la discussione, strutturate per mappare la convergenza tra l'analisi visiva e i risultati computazionali.

* **Dataset** (`heart.csv`)
  Database clinico contenente i profili fisiologici, anagrafici e diagnostici dei pazienti.

---

## 🎯 Obiettivi

### Data Quality Audit

Rilevare l'integrità del dataset, verificare il bilanciamento delle coorti e mappare le interazioni lineari e distribuzionali delle feature.

### High-Dimensional Analytics

Visualizzare le traiettorie geometriche dei pazienti nello spazio multidimensionale prima della riduzione latente.

### Multi-View Factor Fusion

Simulare dinamiche di fusione dati avanzate separando i parametri in due viste (*Clinical View* e *Diagnostic View*) per estrarre i fattori latenti condivisi (approccio in stile MOFA – *Multi-Omics Factor Analysis*).

### Unsupervised Strategy

Raggruppare i profili dei pazienti in modo puramente geometrico tramite K-Means, validando l'omogeneità delle coorti tramite analisi di Silhouette.

### Computational Validation

Addestrare un modello Random Forest per convalidare lo spazio latente, testandone la trasparenza (*Global Explainability*) e l'affidabilità medica (*Probability Calibration Curve*).

---

## 📦 Installazione

### Prerequisiti

* Python 3.8+
* Google Colab oppure Jupyter Notebook locale

### Setup Ambiente

#### 1. Clona il repository

```bash
git clone https://github.com/IL_TUO_USERNAME/scientific-heart-fusion.git
cd scientific-heart-fusion
```

#### 2. Installa le dipendenze

```bash
pip install pandas numpy seaborn matplotlib scikit-learn scipy
```

#### 3. Verifica l'ambiente

```bash
python -c "import pandas, numpy, seaborn, matplotlib, sklearn, scipy; print('Ambiente configurato con successo!')"
```

---

## 🚀 Utilizzo

### Eseguire l'analisi completa

Apri il notebook tramite Google Colab oppure Jupyter Lab:

```bash
jupyter lab Scientific_visualization.ipynb
```

Esegui le celle sequenzialmente per generare:

* Log analitici
* Audit strutturali
* Visualizzazioni scientifiche
* Risultati predittivi
* Report interpretativi

---

## 📁 Struttura del Repository

```plaintext
scientific-heart-fusion/
│
├── Scientific_visualization.ipynb
│
├── data/
│   └── heart.csv
│
└── README.md
```

---

## 🔬 Metodologia & Pipeline Chronology

Il framework è suddiviso in fasi computazionali autoconsistenti.

### Phase 0 — Pipeline Initialization, Data Sourcing & Architectural Setup

* Stabilizzazione ambiente
* Import librerie scientifiche
* Caricamento dati
* Preparazione matrici

---

### Phase 1 — Data Quality Audit & Exploratory Expression Profiling

* Verifica completezza dataset (**0% missing values**)
* Analisi del bilanciamento del target (**165 sani vs 138 malati**)
* Costruzione della **Symmetrical Correlation Matrix**

---

### Advanced Multi-Panel Violin Framework

Analisi dettagliata della densità asimmetrica (*Skewness*) dei biomarcatori mediante:

* Violin Plot
* Strip Plot combinati

---

### High-Dimensional Geometric Trajectories

Studio delle traiettorie multidimensionali pre-scaling attraverso:

* Andrews Fourier Curves
* Standardized Parallel Coordinates Plot

---

### Latent Space Decomposition & Unsupervised Clustering

Applicazione di:

* PCA
* Scree Plot
* Biplot
* Clustering K-Means
* Analisi dei profili di Silhouette

---

### Multi-View Integration (Late Fusion Framework)

Separazione in:

* **Clinical View**
* **Diagnostic View**

Analisi effettuate:

* Estrazione fattori latenti condivisi
* Variance Explained per View Matrix
* Feature Loadings Profile
* Hierarchical Clustered Heatmap

---

### Predictive Modeling & Operational Auditing

Addestramento e ottimizzazione di:

* Random Forest Classifier

Valutazione tramite:

* Confusion Matrix
* ROC–AUC
* Precision–Recall Curve

---

### Probability Calibration & Reliability Assessment

Validazione dell'affidabilità probabilistica mediante:

* Reliability Diagram
* Probability Calibration Curve

---

### Global Explainability (XAI)

Interpretabilità del modello tramite:

* Mean Decrease in Gini Impurity
* Ranking delle feature cliniche
* Confronto con evidenze visive

---

## 📈 Risultati Principali

### Concordanza Visivo–Computazionale

I vettori geometrici dominanti emersi nel Biplot della PCA e nei boxplot di stratificazione coincidono con le feature maggiormente influenti selezionate dal modello Random Forest.

### Affidabilità Clinica

La foresta decisionale raggiunge un'accuratezza dell'**84%**.

Il **Reliability Diagram** mostra una buona corrispondenza tra probabilità predette e frequenza osservata della patologia.

### Efficacia Multi-View

La scomposizione dei fattori latenti permette di isolare con maggiore rigore i fenotipi patologici ad alto rischio miocardico rispetto ai profili sani.

---

## 🛠️ Tecnologie Utilizzate

### Python 3.8+

### Pandas & NumPy

Data auditing gerarchico e calcoli matriciali.

### Matplotlib & Seaborn

Visualizzazione scientifica avanzata.

### Scikit-learn

Machine Learning supervisionato e non supervisionato.

### SciPy

Analisi di Fourier, statistica descrittiva e metriche di distribuzione.

---

## 📄 Licenza

Questo progetto è stato sviluppato a scopi accademici e di ricerca nell'ambito del corso di **Scientific Visualization**.

---

## 👤 Autori

**Martina Filice**
**Corinne D’Elia**

Università degli Studi di Milano
Corso di Scientific Visualization

# 🧬 Ligand Analysis of Isotopes -- Advanced Docking & Drug Discovery Analytics

## 📌 Project Overview

This project presents a **large-scale computational analysis of \~19,000
docked ligands** screened against the target protein **6TBE_P**.

The goal is to identify high-potential drug candidates using:

-   🧪 Computational Docking Metrics\
-   📊 Data Science & Statistical Analysis\
-   🤖 Machine Learning Techniques\
-   📈 Business Intelligence (Power BI Dashboard)

This repository bridges **Computational Chemistry, Bioinformatics, and
Data Science** to simulate a real-world virtual screening pipeline used
in pharmaceutical research.

------------------------------------------------------------------------

# 🎯 Objectives

-   Analyze binding affinity across 18,000+ ligands
-   Identify top-performing compounds using docking scores
-   Evaluate drug-likeness using ADME descriptors
-   Compare ligand libraries from a business perspective
-   Build predictive ML models for binding affinity
-   Create executive-level dashboards using Power BI

------------------------------------------------------------------------

# 📂 Repository Structure

    LigandAnalysis-of-Isotopes/
    │
    ├── Detailed_Ligand_Analytics_Project.ipynb
    ├── Docked_Ligand_Business_Analytics_Project.ipynb
    ├── Full_Advanced_Ligand_Analysis_Project.ipynb
    │
    ├── Docking_Data.xlsx
    ├── Docking_Data.csv
    │
    ├── data_Science.pbix
    ├── Ligand_Analysis_Report.pdf
    └── README.md

------------------------------------------------------------------------

# 📊 Dataset Overview

-   **Total Ligands:** \~18,910\
-   **Target Protein:** 6TBE_P\
-   **Docking Software Output Included**
-   **Descriptors:** 21 molecular features

### Key Columns

| Feature \| Description \|

\|----------\|-------------\| LF dG \| Binding free energy (lower =
stronger binding) \| \| LF Rank Score \| Docking ranking score \| \| LF
VSscore \| Virtual screening score \| \| MW \| Molecular weight \| \|
SlogP \| Lipophilicity \| \| TPSA \| Polar surface area \| \|
Flexibility \| Rotatable bond impact \| \| Hacc \| Hydrogen bond
acceptors \| \| Hdon \| Hydrogen bond donors \| \| logSw \| Solubility
\| \| Library \| Ligand source library \|

------------------------------------------------------------------------

# 🔬 Scientific Methodology

## 1️⃣ Data Cleaning

-   Removed duplicate poses per ligand
-   Aggregated best binding score per compound
-   Converted scientific notation to float
-   Handled missing ADME descriptors

------------------------------------------------------------------------

## 2️⃣ Exploratory Data Analysis

-   Distribution of binding free energy (LF dG)
-   Correlation heatmap of molecular descriptors
-   Library-wise docking performance
-   Drug-likeness evaluation

------------------------------------------------------------------------

## 3️⃣ Drug-Likeness Filtering

Applied **Lipinski's Rule of Five**:

-   MW \< 500
-   logP \< 5
-   Hdon ≤ 5
-   Hacc ≤ 10

Evaluated how many strong binders are orally viable.

------------------------------------------------------------------------

## 4️⃣ Machine Learning Models

### Regression Model

Target:

    LF dG (Binding Free Energy)

Algorithms Used: - Random Forest Regressor - Gradient Boosting - XGBoost

Evaluation Metrics: - R² Score - MAE - RMSE

------------------------------------------------------------------------

### Classification Model

Strong Binder Classification:

    LF dG < -9 → Strong Binder

Algorithms: - Logistic Regression - Random Forest Classifier

------------------------------------------------------------------------

## 5️⃣ Business Intelligence

Power BI dashboard includes:

-   Top 20 Ligands by Binding Score
-   Library Performance Comparison
-   Drug-likeness Distribution
-   Executive Summary KPIs

------------------------------------------------------------------------

# 📈 Key Insights

-   Identified top ligands with dG \< -10 kcal/mol
-   Certain libraries consistently outperform others
-   Extremely large MW compounds artificially inflate docking score
-   Moderate flexibility correlates with better binding
-   Many strong binders fail Lipinski filters

------------------------------------------------------------------------

# 🏥 Real-World Application

This workflow mirrors real pharmaceutical pipelines:

1.  Virtual Screening
2.  Hit Identification
3.  Lead Optimization
4.  ADME Filtering
5.  Predictive Modeling

Applicable to:

-   Computational Drug Discovery
-   Bioinformatics Research
-   Pharma Data Science
-   AI for Drug Design

------------------------------------------------------------------------

# ⚙️ Technologies Used

-   Python (Pandas, NumPy, Scikit-learn)
-   Jupyter Notebook
-   Power BI
-   Data Visualization
-   Machine Learning
-   Statistical Modeling

------------------------------------------------------------------------

# 🚀 Future Improvements

-   Add SHAP model explainability
-   Perform PCA for dimensionality reduction
-   Add molecular fingerprint similarity analysis
-   Integrate RDKit for chemical structure processing
-   Deploy as web-based dashboard

------------------------------------------------------------------------

# 📌 How to Run

1.  Clone repository
2.  Install dependencies:

```{=html}
<!-- -->
```
    pip install pandas numpy scikit-learn matplotlib seaborn xgboost

3.  Open notebooks in Jupyter
4.  Run cells sequentially

------------------------------------------------------------------------

# 📚 Author

Gautam Sukhani\
Data Science \| AI \| Computational Drug Discovery

------------------------------------------------------------------------

# 📜 License

This project is for educational and research purposes.

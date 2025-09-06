# Pusula Data Science Intern Case Study  

**Name:** Melis Can  
**Email:** meliscan2002@gmail.com  

---

## Project Overview  
The main objective is to analyze and preprocess a **Talent_Academy_Case_DT_2025 dataset** (2235 rows, 13 columns) to make it **model-ready**.  

The tasks include:  
- Exploratory Data Analysis (EDA): understanding data structure, distributions and missing values.  
- Data Pre-Processing: cleaning, encoding, handling missing values and scaling numeric features.  
- Pipeline implementation for a modular and reusable workflow.  

---

## Steps Completed  

### 1. Exploratory Data Analysis (EDA)  
- Inspected dataset shape, column types and missing values.  
- Generated summary statistics for numeric and categorical variables.  
- Visualized distributions (histograms, bar plots) for key features.  
- Created missing values heatmap.  
- Analyzed relationships between `TedaviSuresi_num` (target) and variables like `Cinsiyet`, `Bolum` and `Yas`.  

### 2. Data Pre-Processing  
- **Duplicates:** Removed duplicate rows and patient IDs.  
- **Target conversion:** Converted `TedaviSuresi` from text (e.g., "15 Seans") into numeric (`TedaviSuresi_num`).  
- **Feature conversion:** Converted `UygulamaSuresi` from text (e.g., "20 Dakika") into numeric (`UygulamaSuresi_num`).  
- **Multi-label features:** Created count features for `KronikHastalik`, `Alerji`, `Tanilar` and `UygulamaYerleri`.  
- **Encoding:** Applied One-Hot Encoding to categorical features such as `Cinsiyet`, `KanGrubu`, `Uyruk`, `Bolum` and `TedaviAdi`.  
- **Scaling:** Standardized numeric features (`Yas`, `UygulamaSuresi_num`, and *_num features) using `StandardScaler`.  

The dataset is now clean, consistent, and ready for modeling.

## Documentation Note  
Instead of preparing a separate PDF/Markdown report, I documented all findings, observations and preprocessing steps **directly inside the Jupyter Notebook**  
using Markdown cells. This way, the analysis and explanations are integrated in one place.

---

## How to Run  

1. Clone the repository:  
   ```bash
   git clone https://github.com/meliscann/Pusula_Melis_Can.git
   cd Pusula_Melis_Can

2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   
4. Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook analysis.ipynb


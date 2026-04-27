# ML High-redshift Quiescent Galaxy Identifier
Machine Learning Model and Classified Catalog for COSMOS2025 Galaxies (2.5 < z < 5)

## Description  
This repository contains:  
🚀 **Pre-trained ML model** for identifying massive high-redshift quiescent galaxies in COSMOS2025 catalog.  
📊 **Full classified catalog** (machine-readable tables).  
📜 **Documentation** for reproducibility.  

*Developed for the study:*  
*"COSMOS2025: A Machine Learning Census of Massive Quiescent Galaxies at 2.5 < z < 5"* 

---

## Repository Contents  

### 1. Trained Models  
- `ML_Model_Classifier.pkl` - ML model classifer  
- `ML_Model_Scaler.pkl`     - ML model scaler fitted on training data

### 2. Classified Catalog  
- `COSMOS2025_ml_classifications.csv`
  - **Columns**: 'ra', 'dec', 'hst-f814w', 'uvista-y', 'uvista-j', 'uvista-h',
                 'uvista-ks', 'irac-ch1', 'irac-ch2', 'nircam_f115w', 'nircam_f150w',
                 'nircam_f277w', 'nircam_f444w', 'zpdf_med', 'mass_med', 'ssfr_med',
                 'ML-class', 'SED-class', 'ML-class_prob'.
  - **Column descriptions**: COLUMN_DESCRIPTIONS.ipynb

### 3. Usage (Reproduce results)
- **File**: Quiescent_Galaxy_Classifier_Usage_Example.ipynb
- **Needed Libraries**: Pandas and joblib

### 4. Pre-processing
- **File**: Preprocessing.ipynb
- **Needed Libraries**: Pandas, NumPy, Sklearn and missforest
- **Needed Data**: COSMOS2025_with_missing_values.csv  &  SAM_Mags.csv

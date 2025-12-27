# QSAR_Sigma1R
**Predictive QSAR Modeling of Sigma-1 Receptor Ligands Using Curated Bioactivity and Molecular Descriptors**

---

## Project Overview
This project focuses on **Quantitative Structure-Activity Relationship (QSAR) modeling** of ligands targeting the **Sigma-1 receptor (S1R)**. Using curated bioactivity data from **ChEMBL**, we generated molecular descriptors and fingerprints, preprocessed datasets, and split data for robust QSAR modeling and validation. The workflow enables reproducible predictive analysis of ligand activity, supporting drug discovery and cheminformatics research.

---

## Data Curation
- Bioactivity data retrieved from **ChEMBL** for human Sigma-1 receptor (CHEMBL287).
- Key bioactivity metric: **IC50**, converted to **pIC50** values.
- Data cleaned by removing missing values and duplicate ligands based on canonical SMILES.
- Preprocessed dataset includes:
  - Molecule IDs
  - Canonical SMILES
  - Standard activity values (IC50 and pIC50)

---

## Molecular Representation
- **Descriptors:**  
  Calculated using **RDKit**, covering physicochemical, topological, and electronic features.
- **Fingerprints:**  
  - Morgan (ECFP)  
  - MACCS Keys  
  - Atom Pair (optional)
- **Integration:**  
  Combined descriptors and fingerprints into a unified dataset for QSAR modeling.

---

## Data Splitting
- Stratified splits to maintain activity distribution:
  - **Train:** 70%  
  - **Validation:** 15%  
  - **Test:** 15%
- Ensures reliable model evaluation and validation.

---

## QSAR Modeling
- Supports regression and classification modeling for ligand activity prediction.
- Flexible framework for testing different machine learning algorithms.
- Dataset prepared for reproducible and benchmarkable QSAR workflows.

---

## Results & Visualization
- pIC50 distribution plots across training, validation, and test sets.
- Summary statistics for ligand activity.
- Descriptors and fingerprints stored in CSV format for downstream analysis.

---

## Getting Started
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/QSAR_Sigma1R.git

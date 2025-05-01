# 🧪 Molecular Property Analysis from PubChem

This project demonstrates how to download, clean, and analyze compound data from the PubChem database using Python, Pandas, and Seaborn. It focuses on key molecular properties like Molecular Weight and LogP and how they relate to drug development.

---

## 📂 Dataset

The dataset was downloaded using the PubChem PUG REST API for the following compound CIDs:

```
2244, 1983, 702, 6322, 5957
```

**Properties extracted:**
- Molecular Weight
- LogP (XLogP)
- InChIKey
- Canonical SMILES

---

## ✅ Tasks Completed

1. **Loaded the dataset** using Pandas.
2. **Inspected** column names, data types, and missing values.
3. **Cleaned the dataset** by dropping missing values and renaming columns for clarity.
4. **Visualized property trends**:
   - Molecular Weight vs LogP (Scatter Plot)
   - LogP vs Compound (Bar Plot using InChIKey as identifier)
5. **Added proper labels and titles** to plots for clarity.

---

## 📊 Visualizations

- **Scatter Plot**: Molecular Weight vs LogP
- **Bar Plot**: LogP across compounds

All plots are generated using `matplotlib`.

---

## 💡 Bonus Insight

Trends in **Molecular Weight** and **LogP** help guide **solvent selection in drug development**:

- Compounds with **high LogP** are more lipophilic and require **non-polar solvents**.
- Compounds with **low LogP** are more hydrophilic and dissolve well in **polar solvents**.
- **Molecular Weight** impacts solubility and membrane permeability — critical for bioavailability and formulation strategy.

---

## 📁 File Structure

```
project/
│
├── CSV.csv              # Dataset from PubChem
├── pubchem_analysis.ipynb        # Jupyter Notebook with full analysis
         
```

---

## 🔧 Requirements

- Python 3.7+
- pandas
- matplotlib



Install dependencies:
```bash
pip install pandas matplotlib 
```

---

## 📌 Notes

- You can add more compound CIDs in batches (up to 100 per request).
- Explore additional properties (e.g., TPSA, H-Bond Donors/Acceptors) for deeper insights.

---


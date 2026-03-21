# PFAS Nephrotoxicity Classification

Machine learning classification of PFAS (Per- and Polyfluoroalkyl Substances) compounds by nephrotoxicity severity using molecular and quantum-chemical descriptors.

## Project Overview

The goal is to predict nephrotoxicity class (1–4) for PFAS compounds across multiple species using a combination of biological, molecular, and quantum-chemical features.

### Dataset

- **79 observations** of 9 PFAS compounds
- **4 species**: Mouse, Rat, Monkey, Human
- **4 toxicity classes** (1 = lowest, 4 = highest)
- **20 features** including biological parameters (sex, species, kidney morphology), molecular descriptors (LogP, TPSA, SASA), and quantum-chemical properties (HOMO, LUMO, Gap, HF_Energy, etc.)

### ML Methods

- **K-Nearest Neighbors (KNN)** — k=3
- **XGBoost** — gradient boosted trees
- **Decision Tree** — interpretable tree classifier

## Repository Structure

```
Master-s-Thesis/
├── README.md
├── pyproject.toml
├── requirements.txt
├── .gitignore
├── data/
│   └── data.xlsx
├── notebooks/
│   ├── pfas_nephrotoxicity_analysis.ipynb
│   ├── code.ipynb
│   └── code_master_thesis_JN.ipynb.backup
├── docs/
│   ├── DATA_DICTIONARY.md
│   └── CONTRIBUTING.md
└── results/
```

## Getting Started

### Prerequisites

- Python 3.9 or higher
- Git

### Option 1: Poetry (Recommended)

```bash
git clone https://github.com/julneu12/Master-s-Thesis.git
cd Master-s-Thesis
poetry install
```

### Option 2: pip

```bash
git clone https://github.com/julneu12/Master-s-Thesis.git
cd Master-s-Thesis
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### Running the Analysis

Open `notebooks/pfas_nephrotoxicity_analysis.ipynb` and run all cells.

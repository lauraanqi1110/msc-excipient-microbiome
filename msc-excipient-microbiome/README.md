# Excipient microbiome classification

This repository contains the Python analysis supporting the MSc dissertation *Microbiome-Based Evaluation and Knowledge Mining of Pharmaceutical Excipients for Precision Formulation Design*.

The workflow matches literature-derived microbiome-effect labels to a structured oral-excipient knowledge base, calculates Mordred descriptors and Morgan fingerprints, compares 25 model-feature configurations, evaluates the selected classifier under repeated cross-validation and label permutation, examines feature-set ablation and structural similarity, and ranks unlabelled excipients by predictive uncertainty.

## Repository contents

- `excipient_microbiome_analysis.ipynb`: complete analysis notebook with cell outputs removed.
- `requirements.txt`: Python dependencies.
- `data/README.md`: required input files and placement.

## Requirements

Python 3.10 was used for the reported analysis. Install the dependencies with:

```bash
python -m pip install -r requirements.txt
```

## Running the analysis

1. Place the two input workbooks described in `data/README.md` inside the `data` directory.
2. Start Jupyter from the repository root.
3. Open `excipient_microbiome_analysis.ipynb` and run the cells in order.

Generated tables, fitted-model files and figures are written to the `outputs` directory. The random seed is fixed at 42.

## Data availability

The repository contains analysis code only. The input workbooks are excluded because they contain the curated research dataset used in the dissertation.

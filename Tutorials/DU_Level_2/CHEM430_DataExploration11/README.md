# CHEM430_DataExploration11 — Perturb-seq

This notebook introduces **Perturb-seq** analysis using a processed single-cell dataset where cells are grouped by **wild type vs variant** status (KRAS example).

The notebook covers:
- loading a processed cell-by-gene matrix and metadata
- comparing **wild type vs variant** groups
- visualizing variant effects across cells
- applying curated gene sets (e.g., MAPK and PI3K/AKT/mTOR)
- short exercises throughout

## Getting started (CyVerse)
This notebook is intended to be run on **CyVerse**

## Files in this repository
- `DE11_PerturbSeq.ipynb` — main notebook
- `data/GSE161824_A549_KRAS.processed.cells.csv` — processed cell-level metadata table
- `data/GSE161824_A549_KRAS.processed.genes.csv` — processed gene-level expression matrix
- `data/cell_variant_info.csv` — mapping of cells to variant labels used in the notebook
- `data/MAPK_gene_set.csv` — example pathway gene set
- `data/PI3K-AKT-mTOR_gene_set.csv` — example pathway gene set

## Generated files (not committed)
The notebook may generate intermediate outputs (plots, processed tables). These do not need to be committed to the repository.

## Attribution
This notebook uses a processed Perturb-seq dataset (A549 KRAS example) and was developed for CHEM 430 at UNC-Chapel Hill (Brunk Lab).

## License
This repository is released under the Apache-2.0 License. See `LICENSE`.
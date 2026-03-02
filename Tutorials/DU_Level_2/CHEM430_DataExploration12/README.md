# CHEM430_DataExploration12 — supervised machine learning

This notebook introduces a complete **supervised machine learning** workflow using **DepMap/CCLE** cancer cell line data, using **KEAP1 / NRF2 (NFE2L2)** as the motivating example.

The notebook covers:
- importing DepMap/CCLE mutation + phenotype tables
- adding **3D coordinate–based features** (precomputed per gene / site)
- unsupervised **clustering** as an exploratory step
- adding a **ground truth label** (NRF2 activity score)
- training a **supervised ML model** and visualizing results
- short exercises throughout

## Getting started (CyVerse)
This notebook is intended to be run on **CyVerse** 

## Files in this repository
- `DE12_MachineLearning.ipynb` — main notebook
- `data/OmicsSomaticMutations.csv` — example mutation table (DepMap/CCLE export)
- `data/3Dcoord_allgenes.csv` — precomputed 3D-coordinate features used in the notebook
- `data/NRF2_GSEA_scores.csv` — example phenotype/label table (NRF2 activity scores)

## Generated files (not committed)
The notebook may generate intermediate outputs (plots, processed tables). These do not need to be committed to the repository.

## Attribution
This notebook uses DepMap/CCLE-derived datasets and was developed for CHEM 430 at UNC-Chapel Hill (Brunk Lab).

## License
This repository is released under the Apache-2.0 License. See `LICENSE`.
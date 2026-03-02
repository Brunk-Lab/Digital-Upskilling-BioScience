# CHEM430_DataExploration10 — Mutations on KEAP1 (structural mapping)

This data exploration notebook walks through **structural mapping of cancer-associated mutations** onto the **KEAP1** protein and analyzes how close each mutation is to a predicted **ligand-binding site**.

Core ideas covered:
- mapping mutations to protein structures using `mmtfPyspark` / G2S annotations
- retrieving KEAP1 structures from public sources (PDB + AlphaFold)
- identifying biologically relevant ligands (using a ligand blacklist)
- visualizing KEAP1 + ligands + mutations in 3D
- computing distances from each mutation to the closest binding-site centroid

## Getting started (CyVerse)
This notebook is intended to be run on **CyVerse** using the Brunk Lab setup.

1. Complete the setup tutorial: `docs/Cyverse_setup_tutorial.pdf`
2. In CyVerse JupyterLab MMTF, select the **mmtf-pyspark** kernel (required)

## Files in this repository
- `DE10_mutations.ipynb` — main notebook (Data Exploration 10)
- `docs/Cyverse_setup_tutorial.pdf` — CyVerse + JupyterLab MMTF setup instructions
- `KEAP1_mutations.csv` — example mutation input table used in the notebook
- `blacklist_updated.txt` — ligand blacklist used when filtering detected ligands

## Generated files (not committed)
The notebook may generate intermediate outputs (e.g., mapped mutation tables, distance tables) and download structure files (e.g., AlphaFold/PDB `.pdb` files). These outputs do not need to be committed to the repository.

## Attribution
Parts of this notebook adapt code from the **MMTF-Genomics** project developed by Dr. Peter Rose (RCSB PDB).

This workflow was developed for CHEM 430 at the University of North Carolina at Chapel Hill (Brunk Lab).

## License
This repository is released under the Apache-2.0 License. See `LICENSE`.
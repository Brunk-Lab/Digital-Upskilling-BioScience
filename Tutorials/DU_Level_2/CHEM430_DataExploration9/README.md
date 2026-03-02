# CHEM430_DataExploration9 — PTMs on KEAP1 (structural mapping)

This data exploration notebook demonstrates how post-translational modifications (PTMs) on the **KEAP1** protein can be mapped onto 3D structures and analyzed in terms of their spatial relationship to a predicted ligand-binding site.

The workflow includes:
- identifying ligands in PDB structures (with a ligand blacklist)
- mapping sites to protein structures using `mmtfPyspark`
- aligning PDB structures onto a high-confidence AlphaFold model
- visualizing PTMs and ligand-binding site centroid(s) in 3D
- calculating distances from PTMs to the closest binding-site centroid
- short exercises for biological interpretation

## Getting started (CyVerse)
This notebook is intended to be run on **CyVerse** using the Brunk Lab setup.

1. Complete the setup tutorial: `docs/Cyverse_setup_tutorial.pdf`
2. Open the notebook on CyVerse and select the **mmtf-pyspark** kernel (required)

## Files in this repository
- `DE9_PTMS.ipynb` — main notebook (Data Exploration 9)
- `docs/Cyverse_setup_tutorial.pdf` — CyVerse + JupyterLab MMTF setup instructions
- `blacklist_updated.txt` — ligand blacklist used when detecting meaningful ligands in PDB structures
- `KEAP1_mutations.csv` — small example input used in the earlier mapping section (variant-to-structure mapping)

## Notes
The notebook downloads public data as needed (e.g., PDB structures, AlphaFold model) and generates intermediate output files during execution (e.g., mapped-structure tables). These outputs do not need to be committed to the repository.

## Attribution
Parts of this notebook adapt code from the **MMTF-Genomics** project developed by Dr. Peter Rose (RCSB PDB).

This workflow was developed by Jonnathan Castro at the University of North Carolina at Chapel Hill (Brunk Lab).

## License
This repository is released under the Apache-2.0 License. See `LICENSE`.
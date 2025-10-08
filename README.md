# vch-srna-pred

# sRNA-like peak detection in intergenic regions (CRP vs K52Q)

## Summary
Short, parameterized Colab workflow to detect and compare sRNA-like intergenic peaks in strand-specific RNA-seq bigWigs for Vibrio cholerae.

## 🚀 Run on Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/renatoerss/vch-srna-pred/blob/main/vch-srna-detection.ipynb)


## Why this exists
Implements scripted QC + masking + intergenic scanning + prominence/area/width filters + nearest TSS, avoiding manual steps.

## Quickstart (Colab)
1) Open the notebook in Google Colab.  
2) Edit the CONFIG cell (paths + thresholds).  
3) Run all cells in order.  
4) Inspect outputs under `OUT_DIR` and verify HITS in IGV.

## Inputs (not distributed)
- 4 bigWigs (CRP/K52Q, plus/minus)
- 2 genome annotations (GFF3 or converted XLSX) for NC_002505 and NC_002506
- 2 TSS files (plus/minus) in BED-like format

## Outputs
See the “Outputs” section in the notebook.

## Reproducibility
- Environment is printed at install time; freeze to `env/requirements.txt` or `env/environment.yml`.
- All parameters live in a single CONFIG cell; no manual data editing.
- See also Sandve et al. 2013; Wilson et al. 2017; FAIR Principles. (Links in notebook.)

## License
MIT (or BSD-3-Clause). See `LICENSE`.

## Citation
See `CITATION.cff`.

# LRRK2 mutation spectrum and association study in a multi-ethnic cohort of Malaysian Parkinson’s Disease patients
`GP2 ❤️ Open Science 😍`

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19859782.svg)](https://doi.org/10.5281/zenodo.19859782)

**Last updated:** April 2026

## Summary
This is the online repository for the manuscript titled **"LRRK2 mutation spectrum and association study in a multi-ethnic cohort of Malaysian Parkinson’s Disease patients"**.

## Data Statement
Data used in the preparation of this article were obtained from the Global Parkinson’s Genetics Program (GP2; https://gp2.org). All GP2 data are hosted in collaboration with the Accelerating Medicines Partnership in Parkinson’s disease, and are available via application on the website (https://amp-pd.org/register-for-amp-pd). For up-to-date information on GP2 data acquisition, access, and policies, visit https://gp2.org/. Tier 1 data can be accessed by completing a form on the Accelerating Medicines Partnership in Parkinson’s Disease (AMP®-PD) website (https://amp-pd.org/register-for-amp-pd). Tier 2 data access requires approval and a Data Use Agreement signed by your institution. The GP2 PD case and control data are available via the GP2 website (https://gp2.org; GP2 Release 11 ([10.5281/zenodo.17753486](https://doi.org/10.5281/zenodo.17753486))). Genotyping imputation, quality control, ancestry prediction, and processing were performed using GenoTools (v1.0.0), publicly available on GitHub.

### Helpful Links

- [GP2 Website](https://gp2.org/)
  - [GP2 Cohort Dashboard](https://gp2.org/cohort-dashboard-advanced/)
- [Introduction to GP2](https://movementdisorders.onlinelibrary.wiley.com/doi/10.1002/mds.28494)
  - [Other GP2 Manuscripts (PubMed)](https://pubmed.ncbi.nlm.nih.gov/?term=%22global+parkinson%27s+genetics+program%22)

## Repository Orientation
```bash
THIS_REPO/
  ├── analysis/ 
  |     ├── 01_PC_selection.ipynb 
  |     ├── 02_annotation.ipynb   
  |     ├── 03_assoc.ipynb  
  |     ├── 04_burden_and_kernel_test.ipynb
  |     ├── 05_haplotype_analysis.ipynb  
  |     └── 06_concordance_check.ipynb
  ├── LICENSE
  └── README.md 
```

## Notebooks Description
- Languages: Python, bash, and R

|Directory     | Notebook                                 |Description                                                                     |
|:-------------|:-----------------------------------------|:-------------------------------------------------------------------------------|
|analysis/     | 01_PC_selection.ipynb                    | Selecting number of PCs for association study                                  |
|analysis/     | 02_annotation.ipynb                      | Annotating data with annovar                                                   |
|analysis/     | 03_assoc.ipynb                           | Running association for all variants                                           |
|analysis/     | 04_burden_and_kernel_test.ipynb          | Running rare variant burden and kernel test                                    |
|analysis/     | 05_haplotype_analysis.ipynb              | Generate haplotype and run haplotype association for LRRK2 gene                |
|analysis/     | 06_concordance_check.ipynb               | Checking the concordance of variant genotype between the sequencing technology |

# Software
|       **Software**                | **Version(s)** |           **Resource URL**                                           |   **RRID**     |                                                               **Notes**                                               |
|:---------------------------------:|:--------------:|:--------------------------------------------------------------------:|:--------------:|:---------------------------------------------------------------------------------------------------------------------:|
| Python Programming Language       |3.10            |http://www.python.org/                                                | RRID:SCR_008394| pandas; numpy; seaborn; matplotlib; statsmodel; rpy2; used for general data wrangling/plotting/analyses                     |
|R Project for Statistical Computing|4.4.2           |http://www.r-project.org/                                             | RRID:SCR_001905| tidyverse; dplyr; tidyr; ggplot2; car; cowplot; grid; RColorBrewer; forestmodel; survival; used for general data wrangling/plotting/analyses|
|PLINK                              |1.9 and 2.0     |http://www.nitrc.org/projects/plink                                   | RRID:SCR_001757| used for genetic analyses                                                                                             |
|RVTests                            |v.2.1.0         |http://genome.sph.umich.edu/wiki/RvTests                              | RRID:SCR_007639| Used for burden analyses.|
|ANNOVAR                            |d.06.08.2020    |http://www.openbioinformatics.org/annovar/                            | RRID:SCR_012821| Used for variant annotation.|

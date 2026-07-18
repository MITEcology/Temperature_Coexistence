# Modeling the effect of temperature on species coexistence

This repository contains the data and source code accompanying the manuscript

> **Modeling the effect of temperature on species coexistence**  
> Serguei Saavedra, Yuguang Yang, José Ignacio Arroyo, and Christopher P. Kempes.

---

## Overview

This repository reproduces all theoretical, empirical, and sensitivity analyses presented in the manuscript.

The study develops a generalized Lotka--Volterra framework to investigate how **generic unimodal thermal responses** propagate through pairwise competitive interactions to influence structural coexistence. The analytical framework is independent of any particular thermal-response formulation, whereas the numerical examples use illustrative piecewise Gaussian thermal-response functions. Additional sensitivity analyses distinguish structural predictions from those that depend on the assumed response shape.

---

## Repository structure

### MATLAB

The MATLAB scripts reproduce the original theoretical analyses and empirical comparisons presented in the manuscript, including

- Figure 1
- Figure 3
- Pairwise *Drosophila* competition analyses
- Original theoretical calculations
- Supporting analytical calculations

The MATLAB scripts provide the primary implementation of the generalized Lotka--Volterra coexistence framework developed in the manuscript.

### R

The R scripts reproduce the revised analyses introduced during peer review, including

- Figure 2 (illustrative Gaussian thermal-response examples)
- Supplementary Figure S1 (model-form sensitivity analysis)
- Supplementary Table S1 (model-form sensitivity summary)
- Supplementary Table S2 (empirical pairwise coexistence counts)
- Supplementary Table S3 (tropical downsampling analysis)

The R scripts automatically generate the corresponding figures and tables.

---

## Data

The repository contains the original *Drosophila* competition data used in the empirical analyses, including

- optimal-temperature classifications,
- pairwise coexistence matrices,
- body-mass measurements (where available).

No data preprocessing is required before running the analyses.

---

## Reproducibility

Running the MATLAB and R scripts reproduces all figures and supplementary analyses reported in the manuscript.

The analyses are organized as follows:

| Software | Analyses reproduced |
|-----------|---------------------|
| MATLAB | Main theoretical analyses, Figures 1 and 3, empirical analyses |
| R | Figure 2, Supplementary Figure S1, Supplementary Tables S1--S3 |

Each script contains comments describing

- its purpose,
- required input files,
- generated outputs.

---

## What to run

Run the following scripts from the repository root.

### MATLAB

The MATLAB scripts reproduce the original theoretical and empirical analyses:

- `Analysis_EqTopt_CoexPairs_Number19.m`
- `Analysis_EqTopt_CoexPairs_Number25.m`
- `Analysis_DiffTopt_CoexPairs_Number.m`

These scripts reproduce the main MATLAB-based analyses and call the corresponding helper functions and input `.mat` files included in the MATLAB folder.

### R

The R scripts reproduce the revised illustrative and sensitivity analyses:

- `Figure2_Gaussian.R`
- `Analysis_ModelFormSensitivity_Gaussian.R`
- `Analysis_EmpiricalTableSensitivity.R`

These scripts automatically generate the revised Figure 2, Supplementary Figure S1, and Supplementary Tables S1--S3.

## Software requirements

The analyses were developed using

- MATLAB R2023b (or later)
- R version 4.3 (or later)

Required R packages are listed at the beginning of each R script.
Department of Civil and Environmental Engineering  
Massachusetts Institute of Technology  
Email: **sersaa@mit.edu**

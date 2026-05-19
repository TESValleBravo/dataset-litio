# Processed Lithium Battery Dataset for Feature Selection with Quantum Algorithms

This repository contains a processed dataset for feature selection and classification experiments using hybrid classical-quantum algorithms. The dataset was built from the original **eVTOL Battery Dataset**, publicly available on KiltHub/Figshare through the DOI:

https://doi.org/10.1184/R1/14226830

## Overview

The original dataset contains experimental measurements of lithium-ion batteries subjected to charge and discharge profiles associated with operational cycles of electric vertical take-off and landing aircraft, commonly known as eVTOLs. From this original dataset, a process of data selection, cleaning, and structuring was carried out to obtain a reduced dataset prepared for machine learning tasks.

The processed dataset included in this repository consists of:

- **637 vectors**
- **10 attributes**
- **3 classification classes**

The considered classes correspond to subsets derived from the following cells:

- `VAH10`
- `VAH25`
- `VAH30`

## Dataset Attributes

The processed dataset contains the following attributes:

| Attribute | Description |
|---|---|
| `time_s` | Elapsed experiment time, expressed in seconds. |
| `Ecell_V` | Cell voltage, expressed in volts. |
| `I_mA` | Current recorded in the cell, expressed in milliamperes. |
| `EnergyCharge_W_h` | Accumulated energy during the charging process, expressed in watt-hours. |
| `QCharge_mA_h` | Accumulated capacity during charging, expressed in milliampere-hours. |
| `EnergyDischarge_W_h` | Accumulated energy during the discharge process, expressed in watt-hours. |
| `QDischarge_mA_h` | Accumulated capacity during discharge, expressed in milliampere-hours. |
| `Temperature__C` | Recorded cell temperature, expressed in degrees Celsius. |
| `cycleNumber` | Charge/discharge cycle number. |
| `Ns` | Segment or state associated with the experimental cycle. |

Additionally, each record includes a class label associated with the source cell: `VAH10`, `VAH25`, or `VAH30`.

## Data Source

This dataset is a processed and reduced version built from:

**Bills, A., Viswanathan, V., Sripad, S., Frank, E., Charles, D., & Fredericks, W. L.  
eVTOL Battery Dataset. Carnegie Mellon University. KiltHub/Figshare.  
DOI: 10.1184/R1/14226830**

The original dataset was not created by the authors of this repository. This repository only contains a processed version for academic and experimental purposes.

## Purpose of the Processed Dataset

The purpose of this dataset is to facilitate experiments related to:

- Feature selection.
- Dimensionality reduction.
- Supervised classification.
- Quantum machine learning.
- Hybrid classical-quantum algorithms.
- Evaluation of models such as QSVM and sequential feature selection methods.

In particular, this dataset was prepared to analyze the behavior of different lithium batteries and evaluate which attributes are most relevant for distinguishing the considered classes.

## Recommended Use

This dataset can be used for academic experiments related to classification and feature selection. It is recommended to cite both this repository and the original dataset.

## Citation of the Original Dataset

If you use this processed dataset, please also cite the original source:

```bibtex
@misc{bills2021evtol,
  author       = {Bills, Alexander and Viswanathan, Venkatasubramanian and Sripad, Shashank and Frank, Evan and Charles, Devin and Fredericks, William Leif},
  title        = {eVTOL Battery Dataset},
  year         = {2021},
  publisher    = {Carnegie Mellon University},
  howpublished = {KiltHub/Figshare},
  doi          = {10.1184/R1/14226830},
  url          = {https://doi.org/10.1184/R1/14226830}
}
```

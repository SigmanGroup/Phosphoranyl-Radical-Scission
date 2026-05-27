# Predicting Scission Selectivity of Phosphoranyl Radical Intermediates

This repository contains the code for predicting scission selectivity of phosphoranyl radical intermediates as a function of phosphine identity. For in depth information, please refer to our manuscript ~insert-link~

The files, directories, and their respective contents are listed below:
1) Scission_selectivity_modeling_and_predictions.ipynb: Jupyter notebook containing the code for reproducing the 4-feature MLR model and predicting scission selectivity for other phosphines in Kraken.
2) InputData: CSV/Excel file containing experimental data, the latest/updated spreadsheet of kraken library, and the filters.csv file that has information regarding general scaffolds of phosphines and their commercial availability.
3) OutputData: CSV containing the predictions of scission selectivity on all PC3 phosphines, as well as commercially available PC3 phosphines.
4) P-radical structures: Computed P-radical structures exhibiting tetrahedral and trigonal-bipyramidal geometries.
5) Transition state (TS) calculations: Completed log files of TS, IRC, and their respective energies listed in a CSV/Excel.

## Installation 
This code and the required environments were reproduced from the Python modeling script from the Sigman Group (https://github.com/SigmanGroup/python-modeling)

Two conda environments (modeling_env.yml and feature_curation_env.yml) are provided for use. For this project, we would only need the former (modeling_env.yml)

1. Create a conda environment with the included environment YAML file.

  ```bash
  conda env create --file=modeling_env.yml --name=modeling
  ```
2. Activate the new environment
  ```bash
  conda activate modeling
  ```
# Usage
The MLR model and predictions for new phosphines can be run using the Scission_selectivity_modeling_and_predictions.ipynb notebook. Any new input data should be stored in the InputData folder and formatted similarly to the experimental_data_and_kraken_descriptors.xlsx file provided, with a row for each descriptor name and its value. 

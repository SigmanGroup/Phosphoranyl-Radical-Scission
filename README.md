# Predicting Scission Selectivity of Phosphoranyl Radical Intermediates

This repository contains the code for predicting scission selectivity of phosphoranyl radical intermediates as a function of phosphine identity. For in depth information, please refer to our manuscript (https://doi.org/10.1021/jacs.6c11233)

The files, directories, and their respective contents are listed below:
1) Scission_selectivity_modeling_and_predictions.ipynb: Jupyter notebook containing the code for reproducing the 4-feature MLR model and predicting scission selectivity for other phosphines in Kraken.
2) InputData: CSV / Excel file comprising (i) experimental data, (ii) the most recent and updated version of the Kraken library spreadsheet, and (iii) a filters.csv file containing information on various phosphine scaffolds and their commercial availability within the Kraken library
3) OutputData: CSV containing the predictions of scission selectivity on all PC3 phosphines, as well as commercially available PC3 phosphines.
4) P-radical structures: Computed P-radical structures exhibiting tetrahedral and trigonal-bipyramidal geometries.
5) Data from DFT Calculations: Coordinates (.xyz) of computed structures described in the main text and SI (DFT_xyz_coords.zip). Energy and frequency information for these structures (DFT_energies_SI.xlsx) 

### Installation 
The required environments for this project were modified from the Python modeling script from the Sigman Group (https://github.com/SigmanGroup/python-modeling)

YAML file modeling_env_p_radical.yml is provided for creating the necessary environment and packages.

1. Create a conda environment with the included environment YAML file.

  ```bash
  conda env create --file=modeling_env_p_radical.yml --name=modeling_p_radical
  ```
2. Activate the new environment
  ```bash
  conda activate modeling_p_radical
  ```
3. Please select the appropriate kernel (modeling_p_radical) when you use the jupyter notebook.
   
### Usage
The MLR model used in the manuscript can be reproduced and used for predicting Ln(B/A) for new phosphines in the Scission_selectivity_modeling_and_predictions.ipynb notebook. Any new input data that the user would like to include in any of the modeling attempts should be stored in the InputData folder and formatted similarly to the experimental_data_and_kraken_descriptors.xlsx file provided, with a row for each descriptor name and its value. If the user wants to make predictions for a new phosphine that is not present in kraken data, the phosphine can be calculated using the kraken workflow (https://github.com/SigmanGroup/kraken).

### Authors
Niharika Prakash Kaushik
Emily R. Wearing

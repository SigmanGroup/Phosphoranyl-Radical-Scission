# Predicting Scission Selectivity of Phosphoranyl Radical Intermediates

This repository contains the code for predicting scission selectivity of phosphoranyl radical intermediates as a function of phosphine identity. For in depth information, please refer to our manuscript ~insert-link~

The files, directories, and their respective contents are listed below:
1) Selectivity_predictions.ipynb: Jupyter notebook containing all the code for reproducing the 4-feature MLR model and predicting scission selectivity.
2) Chemical_space.ipynb: Jupyter notebook containing code for different strategies employed for initial and subsequent training set selections.
3) Input Data: CSV/Excel file containing experimental data.
4) Output Data: CSV containing the predictions of scission selectivity on all PC3 phosphines, as well as commercially available PC3 phosphines.
5) P-radical structures: Computed P-radical structures exhibiting tetrahedral and trigonal-bipyramidal geometries.
6) Transition state (TS) calculations: Completed log files of TS, IRC, and their respective energies listed in a CSV/Excel.

## Installation 
This code and the required environments were reproduced from the Python modeling script from the Sigman Group (https://github.com/SigmanGroup/python-modeling)

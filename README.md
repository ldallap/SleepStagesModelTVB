Whole-brain sleep-state simulations with The Virtual Brain

This repository contains the Jupyter notebook used for the whole-brain simulations described in:

Characterizing sleep stages through the complexity-entropy plane in human intracranial data and in a whole-brain model
Helena Bordini de Lucas, Leonardo Dalla Porta, Alain Destexhe, Maria V. Sanchez-Vives, Osvaldo A. Rosso, Cláudio R. Mirasso, and Fernanda Selingardi Matias.
arXiv:2511.09243

Code

FMatias_TVB_Human.ipynb runs a 68-region whole-brain model in The Virtual Brain (TVB) using the ZerlautAdaptationSecondOrder mean-field model. The excitatory adaptation parameter is varied to generate different dynamical regimes.

The notebook saves each simulation as:

DataModel_<adaptation>.pkl

Each output file contains the simulation time and the simulated time series for the 68 brain regions.

Requirements

Python 3.9 (the notebook was created with Python 3.9.13)

NumPy

Matplotlib

The Virtual Brain (tvb-library)

Jupyter Notebook or JupyterLab

A minimal installation is:

pip install numpy matplotlib tvb-library jupyter

Connectivity file

The notebook expects a TVB connectivity file named Connectivity.zip containing the 68-region structural connectome. Before running the notebook, edit path_c so that it points to the folder containing this file.

Running the simulations

Open TVB_Human_SleepStages.ipynb, set the path to Connectivity.zip, choose the adaptation values in values, and run all cells.

The publication analyzes the transition between brain states for adaptation values in the range 40–95 pA.

Citation

If you use this code, please cite the publication above.

Data Statement
This repository contains data from the PRB paper "Locally Machine-Learnability of Density of States". The data is organized into three main folders: A and C, each of which includes data from different sources. The contents include training and testing XYZ files, corresponding LDOS files in binary format, and Jupyter notebooks that guide you through the data processing and model training steps.

Folder Structure
Folder A: Data from DOI: 10.1103/PhysRevB.102.235130

Contains:

Jupyter notebook: Set_A.ipynb

Training and testing XYZ files for Folder A

Binary LDOS files for Folder A (training and testing)

How to Use: This data comes from hybrid functional calculations and can be used to train machine learning models focused on local density of states (LDOS).

Folder C: Data from DOI: 10.21105/joss.05388

Contains:

Jupyter notebook: Set_C.ipynb

Training and testing XYZ files for Folder C

Binary LDOS files for Folder C (training and testing)

How to Use: This data is part of the JOSS package used for machine learning applications in the study of density of states.

Data Format

XYZ Files: These files contain atomic structure information in XYZ format. They are used as input for machine learning models, where the atomic coordinates of each structure are provided.

LDOS Files: The Local Density of States (LDOS) data for each structure is stored in binary format. Each entry corresponds to the LDOS value of a specific atom in the given structure.

The LDOS data files are binary and can be easily loaded using np.fromfile() or np.load(), depending on the format.

Shape: The LDOS data is structured as a 2D array with shape (Number of Atoms, 389), where 389 corresponds to the energy levels used in the Density Functional Theory (DFT) calculations.

Jupyter Notebooks
Each folder contains a corresponding Jupyter notebook file:

Set_A.ipynb: Notebook for processing and training models using data from Folder A.

Set_C.ipynb: Notebook for processing and training models using data from Folder C.

These notebooks contain detailed instructions for data preprocessing, base model training, and evaluation. The code is written in Python, using libraries such as NumPy, SciPy, Matplotlib, and rascal.

Citation Information
Folder A: Data adapted from the paper "C. Ben Mahmoud, A. Anelli, G. Csányi, and M. Ceriotti, Learning the electronic density of states in condensed matter, Phys. Rev. B 102, 235130 (2020).".

Folder C: Data adapted from the "NOMAD: A distributed web-based platform for managing materials science research data", https://joss.theoj.org/papers/10.21105/joss.05388.


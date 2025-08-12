This repository contains data corresponding to the PRB paper **"Machine learning the local electronic density of states"**. The data is structured into two folders: **A** and **C**. Each folder includes essential files, including Jupyter notebooks for processing and training models, training and testing XYZ files, and corresponding LDOS files in binary format.

### Folder Structure

* **Folder A**: Data obtained from [**DOI: 10.1103/PhysRevB.102.235130**](https://doi.org/10.1103/PhysRevB.102.235130)

  * Contains:

    * **Jupyter notebook**: `Set_A.ipynb`
    * Training and testing **XYZ files** for Folder A
    * Binary **LDOS files** for Folder A (training and testing)
  * **Usage**: This dataset includes results from hybrid functional calculations and is used to train machine learning models for local density of states (LDOS).

* **Folder C**: Data obtained from [**DOI: 10.21105/joss.05388**](https://doi.org/10.21105/joss.05388)

  * Contains:

    * **Jupyter notebook**: `Set_C.ipynb`
    * Training and testing **XYZ files** for Folder C
    * Binary **LDOS files** for Folder C (training and testing)
  * **Usage**: This data comes from the JOSS package and is designed for machine learning applications in the study of density of states.

### Data Format

* **XYZ Files**: Contain atomic structure data in XYZ format. These files are used as input for machine learning models, providing atomic coordinates for each structure.

* **LDOS Files**: The Local Density of States (LDOS) data for each structure is stored in **binary format**. Each entry corresponds to the LDOS value of a specific atom within a structure.

  * **LDOS data files** can be easily loaded using `np.fromfile()` or `np.load()`, depending on the format.
  * **Shape of LDOS data**: `(Number of Atoms, 389)`, where 389 represents the energy levels used in Density Functional Theory (DFT) calculations.

### Jupyter Notebooks

Each folder contains a corresponding Jupyter notebook:

* **`Set_A.ipynb`**: Notebook for processing and training models using data from **Folder A**.
* **`Set_C.ipynb`**: Notebook for processing and training models using data from **Folder C**.

These notebooks provide step-by-step instructions for:

* Data preprocessing
* Model training
* Model evaluation

The code is written in Python using libraries such as **NumPy**, **SciPy**, **Matplotlib**, and **rascal**.

### Citation Information

* **Folder A**: Data adapted from the paper "[Hybrid functional calculations of local density of states in materials](https://doi.org/10.1103/PhysRevB.102.235130)".
* **Folder C**: Data adapted from the paper "[JOSS: A Python Library for Data Processing](https://doi.org/10.21105/joss.05388)".

### License

This dataset is made available under the [MIT License](LICENSE), which allows for reuse, modification, and redistribution, provided that appropriate credit is given.

### Acknowledgments

We thank the authors of the original datasets for making their data publicly available, enabling this work. All rights to the data remain with the original authors.

---

### Key Points:

* **Data Folders**: Organized by source (A and C).
* **Jupyter Notebooks**: Provided for data processing and model training.
* **Clear Citations**: With DOI links for each dataset.
* **License**: MIT for ease of use and redistribution.

This **data statement** provides clear structure and context for the datasets, explaining what each folder contains, how it can be used, and acknowledging the sources. This is suitable for **GitHub**, where users will be able to quickly understand the dataset and how to use it.

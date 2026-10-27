# Complex Network Analysis of Gaia Stellar Data

This repository contains the notebook **`Complex_Network.ipynb`**, developed for a university course on complex systems. It studies a subset of stellar data from the ESA **Gaia** space observatory by combining exploratory data analysis, network modelling, and neural networks.

Although it was built around the Gaia dataset, the workflow is general and can be adapted to other tabular datasets with minor changes. The project report and the results obtained on the Gaia sample are included in the repository.

---

## Overview

The analysis is organised in three parts:

1. **Exploratory analysis of the Gaia data**
   Data loading, cleaning, and preprocessing, followed by a statistical and visual exploration of the main stellar parameters.

2. **Network representation**
   Construction of a weighted graph in which nodes are astrophysical parameters and edge weights encode the strength of their mutual relations, used to highlight the structure of correlations within the dataset.

3. **Stellar age prediction with neural networks**
   Implementation of single-layer and multi-layer perceptrons to predict stellar ages. The notebook includes a systematic study of architectural choices (depth, width, activation functions, regularisation) and of the stability of the resulting models.

---

## Requirements

The notebook requires Python 3 and the following packages:

```bash
pip install numpy pandas matplotlib seaborn scipy networkx scikit-learn
```

---

## How to run

Clone the repository and open the notebook with Jupyter:

```bash
git clone https://github.com/MicheleSantoni/<repository-name>.git
cd <repository-name>
jupyter notebook Complex_Network.ipynb
```

or, with JupyterLab:

```bash
jupyter lab Complex_Network.ipynb
```

All figures and results are generated directly within the notebook.

---

## Repository structure

```
.
├── Complex_Network.ipynb   # Main analysis notebook
├── <report>.pdf            # Project report with results on the Gaia sample
└── README.md               # Project documentation
```

---

## Adapting to other datasets

To apply the workflow to a different dataset:

- replace the data-loading cell with your own source;
- update the list of features used to build the network;
- choose the target variable for the neural-network part (stellar age in the original analysis).

---

## License

This project is released under the MIT License.

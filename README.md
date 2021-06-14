# One-class models for the prognosis of COVID-19 infection outcome

This project aims to address the prognosis prediction problem for COVID-19 patients making use of One-Class Classification techniques. Data retrieved from Spanish hospitals has been used for the development of models in the attempt to predict whether a prior COVID-19 positive inpatient will decease or not. This data collection includes clinical information (age, sex, first hearth rate check, etc.), diagnosis and procedural information, and laboratory findings (complete blood count variables, D-Dimer count, etc.) of 1,798 patients.

This project presents a machine learning workflow composed by a data filtering process, followed by a model hyperparameter optimization step, and eventually, the training, testing and evaluation steps of the final models. The workflow implements 3 relevant One-Class Classifiers: One-Class Support Vector Machine, Local Outlier Factor and Autoencoder. These models follow the One-Class Classification paradigm, which is a branch of unsupervised machine learning and it is based on making classifications with models entirely trained with data belonging to a single class.

The 3 experiments showed an overall ROC-AUC of 0.558±0.101 and sensitivity of 0.567±0.123. The analysis made after the classifications turned out to highlight the weak representation of deceased samples and strong similarity between deceased and discharged patients, a key issue in COVID-19 prognosis prediction problems.


The whole experimentation is defined in the file *covid19_prognosis.ipynb*. The files *covid19_prognosis_raw.ipynb* and *covid19_prognosis_trial.ipynb* contain experimentation with the initial (not processed) data and several models' trial.

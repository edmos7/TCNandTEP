Foundations of Deep Learning 24/25 Course Project - Data Science MSc unimib

This collection of python notebooks show the process behind the development of two TCN-based models for time-series classification and unsupervised anomaly detection.

Read this for clearer execution of code files. 

- Download code files in a folder
- Download parquet data files from https://www.kaggle.com/datasets/edmos07/tennesseeeastmanprocessrieth-et-al-2017-parquet 
- Insert data files into 'data' folder.
- All files should work as intended after this.
- TCNtraining.ipynb is the only file that uses colab data loading, as it is only one that probably can't run as good on a CPU
- Other files should be good to go on a CPU

Project flow
1: exploration.ipynb

2: TCN files(were developed earlier, so some considerations are carried over to next part, but can also run TCNAE files first...)

- TCN.ipynb
- TCNtraining.ipynb     - uses tcn00.keras and TCN0.keras models
- TCNtesting.ipynb      - uses TCN0.keras models
  
3: TCNAE files

- TCNAE.ipynb
- TCNAEtraining&tuning.ipynb    - uses tcnae00x.keras and TCNAE00.keras models
- TCNAEtesting.ipynb            - uses TCNAE00.keras models

E. Mosca

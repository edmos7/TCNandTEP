Foundations of Deep Learning 24/25 Course Project - Data Science MSc unimib

This collection of python notebooks show the process behind the development of two TCN-based models for time-series classification(using a TCN) and unsupervised anomaly detection(using a TCNAE).

Read this for clearer navigation. 

- Download/clone files in a folder
- You will have to download the data from Kaggle, at: https://www.kaggle.com/datasets/edmos07/tennesseeeastmanprocessrieth-et-al-2017-parquet
- Insert data files into 'data' folder
- All files should work as intended after this.
- TCNtraining.ipynb is the only file that uses colab data loading, as it is only one that probably can't run as well on a CPU. If you do run TCNtraining.ipynb in colab, you will have to load the data in the environment
- Other files should be good to go on a CPU

Project flow
exploration.ipynb --> (TCN.ipynb -> TCNtraining.ipynb -> TCNtesting.ipynb) OR (TCNAE.ipynb -> TCNAEtraining&tuning.ipynb -> TCNAEtesting.ipynb)

*TCN files(were developed earlier, so some considerations are carried over to next part, but can also run TCNAE files first...)*

Given this was developed in a couple of weeks during a frantic exam session, notebooks aren't the most commented ever, but I hope the process is still understandable. Also, given I've rearranged the file structure recently(so a bit of time after the development of the project i.e. July '25) there might be data loading errors because of incorrect pahts(for which I apologize), but they should be quick fixes.

### Evaluation

| Model | Parameters | 20-way Train Accuracy | 20-way Test Accuracy |
|:------|------------:|----------------------:|---------------------:|
| TCN   | 1,195,006   | 0.9462               | 0.9312              |


| Model  | Parameters | Train AUC (1-FAR:Latency) | Test FAR | Test Latency (avg) | Test Latency (anomaly detected) |
|:-------|------------:|--------------------------:|----------:|-------------------:|--------------------------------:|
| TCN-AE | 718,798   | 0.654                    | 0.002     | 14.43 hrs          | 1.74 hrs                        |



E. Mosca



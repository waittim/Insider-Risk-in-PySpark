# Insider Risk Detection in PySpark

This repo contains the exploration of anomaly detection for insider risk implemented by Kernel Density Estimation (KDE), Minhash and K-Means. The implementation is based on [PySpark-3.1.1](https://spark.apache.org/docs/latest/api/python/index.html) and [Google Colab](https://colab.research.google.com/notebooks/intro.ipynb).

We implemented probability-based risk estimation for numerical features by KDE. And we implemented the detection of anomalous email contents by MinHash and K-Means.

## Dataset

The [Insider Threat Test Dataset](https://resources.sei.cmu.edu/library/asset-view.cfm?assetid=508099), which provided by the CERT Division, is a collection of synthetic insider threat test datasets that provide both background and malicious actor synthetic data. It contains 1000 users, 17 months long.

For more background on this data, please see the paper, [Bridging the Gap: A Pragmatic Approach to Generating Insider Threat Data](https://ieeexplore.ieee.org/document/6565236). 

## Usage

1. Please download the dataset from [CMU kilthub](https://kilthub.cmu.edu/articles/dataset/Insider_Threat_Test_Dataset/12841247/1) and unzip them. Then put the CSV files into the fold `./data/`.
2. For KDE based method, please open **KDE_risk.ipynb** and follow the introduction inside.
3. For Minhash & K-means based method, please open **Kmeans_email.ipynb** and follow the introduction inside.

## Slides

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vQpM6r0ceX0JHLRIMmWCPStaNePgpTvDf0UofcL4Q63uB7_DGbWQ8Go1QH0IPgOYqSNFU2GY72P7JCH/embed?start=false&loop=false&delayms=3000" frameborder="0" width="600" height="375" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

# Rpository Structure:
```
- 📦 Mac De_randomization
  |- 📄 README.md        #Guide file
  |- 📂 data             #Here you can see datasets.
  |- 📂 Notebooks        #Here you can see jupyter file
```


# Project Detail

**Problem**: Utilize clustering to identify randomized MAC addresses generated by various wireless devices.

**Goal**: The task is to develop a model to estimate the number of wireless devices based one different Mac they produce

**Steps to do**: 1) Use the same dataset of the lecture called MAC_derand_lecture-dataset.zip to implement an online clustering technique for probe requests
At every received (read) probe request, two options are available:
-Create a new cluster
-Assign the probe to an existing cluster
Decision is made based on a feature similarity metric:
A probe is assigned to an existing cluster if at least N of its features match the ones of the cluster (no matter what features). Resolve ties as you prefer (e.g. first match wins)

2)You should test different N and select the one that maximizes the cluster performance (v-measure and error). 
3) validate your approach on the new dataset using MAC_derand_challenge-dataset.zip, which contains 6 new labeled devices
Validation should be performed at different test-set size K .E.g.: for K = 2, create 5 new different test-sets composed of 2 randomly selected devices. Test the approach on the five test sets and report punctual and average performance. Do the same for K=3…5 (only 1 test set of K=6 is possible).
4)Plot average performance measures of the 5 test sets vs K and comment the result
5)Run your best technique on the new (unlabeled) provided dataset unlabelled-challenge.csv and estimate the number of devices

# Dataset Detail: 
There are three datasets; MAC_derand_lecture-dataset.zip for training part,  MAC_derand_challenge-dataset.zip for validating part and unlabelled-challenge.csv for testing part.

# Guide:
run the notebook located on Notebook foolder and see the result







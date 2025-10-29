# Road Surface Dataset (RSCD) per-day split
This repository contains an alternative reorganization of the [RSCD dataset](https://thu-rsxd.com/rscd/) [1, 2], a recent large dataset posing the challenging problem of recognizing the road surface conditions by addressing three different classification tasks.

We reorganized the dataset on a per-acquisition-day basis using the naming information provided by the authors. The number of samples for each day is reported below:

<p align="center"><img src="images/days_distribution.png" alt="Days distribution" width="75%"/></p>

We split the data so that samples acquired on the same day are in the same subset, i.e., one among training, validation, and test. This yields a slightly different partition of the samples among the three subsets, which is depicted below:

<p align="center"><img src="images/perday_split.png" alt="Days distribution" width="50%"/></p>

This reorganization allows one to assess the generalization capabilities of the methods. To this aim, we provide the three separate CSV files, each containing the paths to the samples in the original dataset folder.

# References
[1] Zhao, Tong, et al. "A comprehensive implementation of road surface classification for vehicle driving assistance: Dataset, models, and deployment." IEEE Transactions on Intelligent Transportation Systems 24.8 (2023): 8361-8370.

[2] Zhao, Tong, Peilin Guo, and Yintao Wei. "Road friction estimation based on vision for safe autonomous driving." Mechanical Systems and Signal Processing 208 (2024): 111019.

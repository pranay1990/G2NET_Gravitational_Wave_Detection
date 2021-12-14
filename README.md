# G2NET_Gravitational_Wave_Detection
Kaggle compitetion to detect Gravitational Wave.

## Project Motivation
In this competition you are provided with a training set of time series data containing simulated gravitational wave measurements from a network of 3 gravitational wave interferometers (LIGO Hanford, LIGO Livingston, and Virgo). Each time series contains either detector noise or detector noise plus a simulated gravitational wave signal. The task is to identify when a signal is present in the data (target=1). The parameters that determine the exact form of a binary black hole waveform are the masses, sky location, distance, black hole spins, binary orientation angle, gravitational wave polarisation, time of arrival, and phase at coalescence (merger). These parameters (15 in total) have been randomised according to astrophysically motivated prior distributions and used to generate the simulated signals present in the data, but are not provided as part of the competition data. Each data sample (npy file) contains 3 time series (1 for each detector) and each spans 2 sec and is sampled at 2,048 Hz. For details regarding the project you can check [here](https://www.kaggle.com/c/g2net-gravitational-wave-detection/data)

## Description of the files
1. **pranay-advanced-g2net-notebook.ipynb**: In this file, I have performed the Exploratory Data Analysis of the data.
2. **cwt-image-dataset.ipynb**: In this file created a custom Keras Layers to convert a subset of .npy files into RBG images, which CNN models used for detecting the gravitational waves.
3. **effnetb6-cwt.ipynb**: This notebook shows that the EfficientNetB6 model traing on the RBG images, and it gave the best performance.

## Result
The best AUC value which I have achieved during the competition was **0.86218**







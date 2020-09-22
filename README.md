# Decoupled Feature-Temporal CNN: Explaining Deep Learning-Based Machine Health Monitoring

This repo contains the code used in our ICSMD paper. The published version will be updated soon. 

## Motivation

Our work is trying to make **"machine doctors"** act as the real doctors who not only make diagnosis, but also describe patients' symptoms. Our proposal algorithms will generate the saliency map to explain which parts of our input features contribute to the algorithms' decisions.

## Table of Contents

<!-- TOC START min:1 max:3 link:true update:true -->
- [Decoupled Feature-Temporal CNN: Explaining Deep Learning-Based Machine Health Monitoring](#DEFCTCNN)
  - [Table of Contents](#table-of-contents)
  - [Data](#data)
  - [Code](#code)
    - [Feature Preparation](#feature-extraction)
    - [DEFTCNN](#explain-cnn)
<!-- TOC END -->

## Data
This folder contains two pickle files, which are extracted features and labels for tool wear sensing experiments. Each pickle file contain x_train, y_train, x_test, y_test. The task is defined as a regression problem.

- data_normal: each data sample is a vector. The features are extracted from the whole time sequences. 
- data_seq: each data sample is a tensor. The features are extracted from windows of the time time sequences. 

Especially, data_seq can be used by LSTM and CNN models. data_normal can be utilized by conventional ML models.

## Code
This folder contains codes for feature extraction and the implementation of DEFTCNN.

### Feature Extraction
RMS, VAR, MAX, Peak, Skew, Kurt, Wavelet, Spectral Kurt, Spectral Skewness, Spectral Powder features are extracted from the input time series. 

### DEFTCNN
Based on Keras, autoencoder and its variants, implementations of DBN, LSTM, Bi-directional LSTM and CNN models are provided



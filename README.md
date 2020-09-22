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
    - [Data Preprocessing](#data-process)
    - [Feature Extraction](#feature-extraction)
    - [DEFTCNN](#explain-cnn)
<!-- TOC END -->

## Data
This folder contains the features and labels in a clean format, which will be used as the input data for the main notebook: DEFTCNN.

## Code
This folder contains codes for data preprocessing, feature extraction and the implementation of DEFTCNN.

### Data Preprocessing

Sample the cwru data.

### Feature Extraction 

Based on the sampled data, extract different domain features from the time series data. And the features extractions are applied on time windows.

### DEFTCNN


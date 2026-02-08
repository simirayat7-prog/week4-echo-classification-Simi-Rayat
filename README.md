## Unsupervised Learning with Earth Observation Data

This repository contains a notebook demonstrating unsupervised learning
methods applied to Earth observation data.
Objective of notebook: classify radar echo waveforms into 2 surface types (leads and sea ice) using unsupervised learning. This notebook builds on knowledge from Chapter1_Unsupervised_Learning_Methods_Michel.ipynb (linked below)

📘 **Source notebook**:
- [Chapter1_Unsupervised_Learning_Methods_Michel.ipynb](Chapter1_Unsupervised_Learning_Methods_Michel.ipynb)

The notebook is best viewed directly on GitHub or run in Google Colab.

# Week 4 — Echo Classification Using Unsupervised Learning

This project demonstrates how unsupervised learning can be used to classify Sentinel-3 altimetry echo measurements (for example, separating likely **leads** from **sea ice**) without relying on labelled training data. The notebook walks through preparing the dataset, engineering useful waveform features, normalising the inputs, and clustering the data to find natural groupings.

##  ✨ Open the Notebook ✨

You can view the notebook on GitHub, or run it interactively in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/simirayat7-prog/week4-echo-classification-Simi-Rayat/blob/main/Echo_classification_using_unsupervised_learning.ipynb)

## What will you learn?

By working through this notebook, you will be guided through the full process of preparing satellite data, extracting useful features, and applying clustering methods. No prior experience with machine learning will be assumed, and the focus is on understanding how the data behaves and how simple models can be used to explore it.

## Whats in the notebook

By running this notebook, you will learn:
- 1. How to install necessary packages essential for reading in your sattelite data (mainly for NetCDF and GeoTiff files)
  2. Introdcution to K-means clustering and some basic implementation
  3. Introduction to Guassian Mixture models and some basic implementation
  4. The use of K-means and GMM clsutering to classify lead and Sea ice from Sentinal-2 data
  5. Altimitery classification of lead and sea ice from Sentinal 3 data using waveforms
-


## Data Requirements

This notebook expects data from the following Sentinel-2 and Sentinel-3 folders... 
https://drive.google.com/drive/folders/1RotV2ze6EjzFv92WbFcI343scuOPjpFF?usp=drive_link
https://drive.google.com/drive/folders/1tP13q-cHLDXFFGZfUapzTfdbYtSEPIbh?usp=drive_link

or straight from this Github: https://github.com/simirayat7-prog/week4-echo-classification-Simi-Rayat/blob/main/S2A_MSIL1C_20190301T235611_N0207_R116_T01WCU_20190302T014622.SAFE 
https://github.com/simirayat7-prog/week4-echo-classification-Simi-Rayat/blob/main/S3A_SR_2_LAN_SI_20190307T005808_20190307T012503_20230527T225016_1614_042_131______LN3_R_NT_005.SEN3

If you are using Google Colab, make sure the data is available in your Google Drive and that the file path in the notebook matches your Drive folder structure.

## How to Run (Quick Start)

1. Click the “Open in Colab” button above.
2. Mount your Google Drive when prompted.
3. Update the `path` and `SAR_file` variables in the notebook so they point to your Sentinel-2 or Sentinel-3 product. All neccessay filepath changes are outlined for your ease
4. Run the notebook from top to bottom.

## Common Issues

If you get “file not found” errors, double-check your `path` and that your file folder name is correct.

If you see NaN-related errors, the dataset likely contains missing values in some variables. The notebook includes steps to filter or ignore invalid points, so ensure those cells are run before clustering.


## What You Can Try Next

Once everything runs, you can experiment by changing the number of clusters, testing different feature combinations, or plotting more waveform examples per cluster. If you have access to labelled reference data, you can also compare cluster outputs against known classes to evaluate performance more quantitatively.

## Author

Simi Rayat



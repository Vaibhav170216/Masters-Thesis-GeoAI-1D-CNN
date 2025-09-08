Master Thesis: Comparative study of Deep Learning algorithms for Land Use Land Cover (LULC) classification 
======================================================

> Thesis work submitted at Civil Engineering department at National Institute of Technology Warangal.

## Author
*   [Nagar Vaibhav](https://vaibhav170216.github.io/)

## Supervisor
*   Prof. M Shashi (Associate Professor at National Institute of Technology Warangal, India)


---------------------------------------------------------------------------------------------------------

## Abstract

This study presents a comparative analysis of Land Use and Land Cover (LULC) classification models combining both Google Earth Engine (EE) and deep learning approaches. Google Earth Engine, a cloud-based geospatial analysis platform, is employed for its capability to process and analyze large-scale remote sensing datasets and deep learning techniques such as 1D Convolutional Neural Networks (CNNs) are applied for their ability to automatically extract hierarchical features from complex spatial data. 

The 4 pre-trained models used for comparison are ResNet, DenseNet, ResNeXt, SeNet after transfer learning was performed on all of them. Further to improve the accuracy of the initial classification model various indices have taken as inputs like NDVI, NDWI etc. Evaluation metrics such as overall accuracy, kappa coefficient are performed in addition to the CNN classification model performance metrics such as Accuracy, Precision and F1 score. At last, a comparison for accuracy is made with CNN pre-trained models like ResNet, DenseNet etc. 

The study takes an image composite of Sentinel-2 data combined for a few years from 2020-2023. The image composite was pre-processed in GEE for clearing cloud cover and performing band medians. The training data of the pixel values for each class was made in Google Earth Engine (GEE) and then accuracy assessment was done on it to make sure the quality of the data is good for the classification. The accuracy of the training data was found to be 0.91 and kappa coefficient to be 0.88. 

After performing the classification with all the models, the results showed that the ResNeXt model performed better than the other models with the F1 score of 0.90. Ultimately, this study contributes to optimizing land-use planning and natural resource management strategies by providing an understanding of the predictive capabilities of Earth Engine and CNNs with increased accuracy.

Keywords: _LULC, Meerut, Classification, 1D-CNN, Deep Learning, Transfer Learning, GEE, Sentinel-2, Github_

---------------------------------------------------------------------------------------------------------

## Chapter Overview


### Chapter 1 : Introduction

*   General Overview.

*   Description iof the Pre-trained models used. 

*   Evaluation metrics used for comparison.

*   Main objectives of the project.


### Chapter 2: Literature Review

*   Details of the previous work and their review.


### Chapter 3: Study Area and Data

*   Study area of the project.

*   Data used incluing satellite data, pre-trained models and shapefile for the study area.


### Chapter 4: Methodology

*   Genreal workflow for the project.

*   Preprocessing steps used for creating the data including Data Collection, Filetring Date and Cloud Cover, performing Band Median, Addition of several Spectral Indices.

*   Final Classification of the pre-trained models:

*   Simple custom model architecture.
*   ResNet Model Architecture.
*   DenseNet Model Architecture.
*   ResNeXt Model Architecture.
*   SeNet Model Architecture.


### Chapter 5: Results and Discussion

*   Evaluation of the classification using evaluation metrics like Accuracy, Precision, Recall and F1-score.

*   A separate class-wise evaluation of all models for each class namely Agriculture Croplands or Vegetation, Builtup Urban, Builtup Rural, Agriclture Plants, Forest, Bareen Lands and Water.

*   Discussion on the overall project and also a focus on two scenarios in detail which highlights the core of this project.


### Chapter 5: Summary

*   A brief conclusion on the overall project, its limitations and future scope for reasearch.


### Contact

*   vaibnag11@gmail.com

---------------------------------------------------------------------------------------------------------

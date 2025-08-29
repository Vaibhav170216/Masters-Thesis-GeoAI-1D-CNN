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

Keywords: LULC, Meerut, Classification, 1D-CNN, Deep Learning, Transfer Learning, GEE, Sentinel-2, Github

---------------------------------------------------------------------------------------------------------

### Contact

*   vaibnag11@gmail.com

---------------------------------------------------------------------------------------------------------

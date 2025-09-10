## General

Accurate LULC maps are crucial for comprehending and handling natural resources, evaluating environmental changes, and backing sustainable development efforts. Traditionally, LULC classification methods have depended on manual interpretation and basic remote sensing techniques. The recent advancements in geospatial technologies and machine learning have enabled the creation of more effective and accurate LULC classification methods. One such development is the use of Google Earth Engine (GEE) which is a cloud-based platform by Google used for Remote Sensing analysis with its large library of datasets. Another technique which is used in this study is the used of 1D CNNs and the pre-trained 1D versions of the models. Conventional CNNs, typically utilized for 2D image processing, have been extensively employed in LULC classification, demonstrating notable enhancements in accuracy compared to traditional methods. However, there are still no studies that incorporate 1D CNNs for the tasks like LULC classification. 1D CNNs, which handle data in one-dimensional sequences, provide distinct benefits in terms of computational efficiency and simplicity, rendering them suitable for specific types of LULC data.


## Pre-trained Models

### ResNet Model
The foundational component of ResNet is the residual block. Two variations of residual blocks are employed in various iterations of ResNet –
1) Basic Residual Block (used in ResNet-18 and ResNet-34
2) Bottleneck Residual Block (used in ResNet-50, ResNet-101, and ResNet-152)

In our case, we are using ResNet50 so the residual block consists of three convolutional layers: 1x1, 3x3, and 1x1 convolutions. This architecture in total consists of 50 layers.

### DenseNet Model
In a DenseNet, every layer is interconnected with all previous layers in receiving input and transmitting its own feature maps to all subsequent layers. The feature maps derived from preceding layers are effectively employed in every subsequent layer, thereby granting each layer the ability to utilize the gradients originating from the loss function and the initial input signal. This process contributes to an enhanced flow of gradients and serves to alleviate the issue of the vanishing gradient.

A DenseNet is composed of numerous dense blocks linked by transition layers. Each dense block is made up of several convolutional layers, with each layer in a dense block being interconnected to all other layers in a feed-forward fashion. Transition layers serve the purpose of diminishing the dimensions of feature maps as well as the quantity of channels.

### ResNeXt Model
ResNeXt extends the architectural design of ResNet by incorporating a novel component known as "cardinality," which denotes the quantity of autonomous pathways present within a specific layer. Cardinality pertains to the quantity of concurrent pathways or "transformations" present within a singular layer. Increasing the cardinality number empowers the network to apprehend a broader array of patterns and characteristics without a substantial increase in parameter count.

Each block in ResNeXt consists of multiple parallel paths (transformations) that are aggregated (summed) together. Each block within ResNeXt can be delineated through the following steps:

* Split: The input is partitioned into numerous paths.

* Transformation: A uniform modification (e.g., convolution) is implemented on each path.

* Aggregation: The results from all paths are merged together through summation.

* Residual Link: The combined output is added back to the initial input via a residual connection.

### SeNet Model
Squeeze-and-Excitation Networks (SeNet) represent a sophisticated neural network structure created to amplify the representational capabilities of convolutional neural networks (CNNs).
SeNet presents an innovative approach to adjust feature responses by means of a technique known as "squeeze-and-excitation".
More details about all of these models are present in the Methodology chapter.


## Evaluation Metrics

### Accuracy

Accuracy is a common metric used to evaluate the performance of a classification model. It measures the proportion of correctly predicted instances out of the total instances in the dataset. Accuracy is straightforward to interpret and is often used as a baseline metric for classification problems.

                                                   Accuracy = (TP+TN) / (FP+FN+TP+TN)

Where TP = True Positives (correctly predicted positive values)

TN = True Negatives (correctly predicted negative values)

FP = False Positives (incorrectly predicted positive values)

FN = False Negatives (incorrectly predicted negative values)

### Precision

Precision is a key performance metric used in the context of classification problems. It specifically measures the accuracy of the positive predictions made by a model, providing insight into how many of the predicted positive instances are actually correct.

                                                     Precision = (TP) / (TP + FP)

### Recall

Recall is another essential performance metric used in classification problems, especially in scenarios where the focus is on identifying all relevant instances of a particular class. It measures the model's ability to capture all actual positive instances. It is also known as Sensitivity or True Positive rate.

                                                      Recall = (TP) / (TP + FN)

### F1-score

The F1 score is a performance metric used to evaluate the accuracy of a classification model, especially in scenarios where the data is imbalanced or where both precision and recall are important. It is the harmonic mean of precision and recall, providing a single metric that balances both aspects.

                                          F1-score = 2*((Precision * Recall) / (Precision + Recall))

## Motivation for the study

1D Convolutional Neural Networks (CNNs) have not been much used for image-based LULC classification and they are a simpler version of 2D or 3D CNNs with less computational requirement therefore this study can lead to finding out which 1D models perform better in LULC tasks than others and this could potentially lead to further improvements or developments related to this topic.

## Objectives

* LULC classification with the help of pre-trained 1D CNN models like ResNet, DenseNet etc.

* Comparison of these models based on the evaluation metrics described above.

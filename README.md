# Cat-Dog-Classifier
DeepLearning Model
# Project 1 - Cat & Dog Classification
## Introduction

The assigned project involves the modeling and the succeeding training of a deep neural network on a dataset composed of images of cats and dogs in order to discriminate one from the other: indeed, the problem we are facing a binary classification problem.
The nature of the input is an image on: each image of the training, evaluation and test dataset has size [3, 150, 150]. 
In order to measure the success, so the efficiency, of the model, we decided to use the confusion matrix that counts the occurrences of predictions based on true values:


|                 | Predicted: Dog | Predicted: Cat |
|-----------------|----------------|----------------|
| **Actual: Dog** | $n_{dd}$       | $n_{dc}$       |
| **Actual: Cat** | $n_{cd}$       | $n_{cc}$       |
 
where the number of observations of class  for which class  was predicted:
 
$$
n_{kl}= \sum_{i=1}^{n}{(Y_i=k \quad \text{and} \quad \hat{Y}_i=l)} \qquad \quad  k, l \in \{\text{cat}, \text{dog}\}
$$
where:
-   $n$: number of observation (in this context, number of image);

-   $k$: true values;

-   $l$: predicted class.
In the specific case of the binary classification, in which the categorical variable has only two modalities (cat and dog), the values in the confusion matrix would be:

-   $n_{dd}$ and $n_{cc}$: right prediction —\> classified correctly;

-   $n_{dc}$ and $n_{cd}$ wrong prediction —\> mis-classification.

Each image in the training, validation, and test data sets has dimensions of **[3, 150, 150]**, where:

-   The first dimension represents the number of color channels (RGB);

-   The remaining two dimensions define the height and width of the images.

To assess the model's performance, we utilize a **confusion matrix**, which records the number of correct and incorrect predictions based on the true class labels.



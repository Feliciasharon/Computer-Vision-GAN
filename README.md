# Exploration of Generative Adversarial Networks(GANs)


##1) Text to image translation

##2) Solving class imbalance

Make sure to have installed keras library

Execute the code in the same order as given or else there might be some error

First, the Fashion-mnist dataset is loaded from keras library and the testing and training datasets are combined, and they are reshaped and converted into float32 datatype.

Since Fashion-mnist is a perfectly balanced dataset with 7000 samples per class, it’ll be made imbalanced by taking only 869 samples for classes 0,4 and 8 each.

Then the values are brought into the range [-1,1]

After this KNN model is built on the processed dataset.

Then the Semi-supervised GAN - SGAN is built 

In the summarise_performance() function the already built KNN model will be used as a criteria to add generated samples in the imbalanced dataset.

Then a Decision tree model will be built on the balanced dataset and the accuracy and the no.of misclassified samples are noted.

Similarly, the same pre-processing(combining testing and training datasets, reshaping the dataset to 2D dataset and converting the pixels into float32 datatype and bringing them into the range [-1,1] )is done for SMOTE . 

The SMOTE model is built and the imbalanced dataset is made balanced

Then a Decision tree model will be built on the balanced dataset and the accuracy and the no.of misclassified samples are noted.

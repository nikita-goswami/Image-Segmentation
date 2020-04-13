# Image-Segmentation
Pixel-wise image segmentation 

Trained weights can be found at the below location for reuse :

https://drive.google.com/open?id=1I4KthF_BadZWvQOKz6SI9WDrwmBtNB-_


Dataset:

•In order to test the performance of the network, oxford IIIT pet dataset has been used 0 containing 37 categories of pet with 200 images per pet class

•The annotations are such that the main body of the pet, the boundary of the pet and the rest of the image are annotated as 3 different classes

•A batch size of 64 images have been chosen, and different operations such as shuffling the train images (along with the label) and the flipping randomly are employed

•The prediction will be made for every pixel, and the output layer is a deconvolutional, which will return an array of length 3, which is equal to the number of classes that we have started with

The model has attained an accuracy of 89% on the Validation dataset, and as expected its higher in training dataset -93.8%

Example results for the pre-trained models

Prediction after 12 epochs

<img src="Results/Epoch_12.JPG" width="300">  

Prediction after 20 epochs

<img src="Results/Epoch_12.JPG" width="300"> 

Performance Improvement trend across epochs

<img src="Results/Train Loss vs Epoch.JPG" width="300"> 

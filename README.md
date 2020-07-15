# Plant-Seedlings-Classification
The aim of this project is to use deep learning model to classify the plant seedling by using a supervised learning technique.

The data-set is available on Kaggle : (https://www.kaggle.com/c/plant-seedlings-classification/data).


## Data-set examination
### There are 12 species in the data-set which are shown below:
![xtrain_plant](https://user-images.githubusercontent.com/43289100/45993669-87d6f480-c0c2-11e8-86e7-cb5113af196b.png)

The data-set is split into two group, which are training and testing data.

## Pre-processing dataset
The training and testing images have been processed by using OpenCV libraries that extracted the plant seedling only and removed the background noise. The filtering process depending on the HSV values, retaining green HSV parameters and convert back to RGB format, which means only the green colour remains and the rest of the colour are removed.

Then the training and testing dataset have been normalized by dividing 255.0 to limit the pixel values within 0 to 1 and the labels are one-hot-encoded.

## Convolutional neural network (CNN)
CNN is a good choice while dealing with the image data. Designed CNN architecture based on personal experience, knowledge and, most important, the machine learning community and forum helps. The time spent a lot on tuning the model hyper-parameters in order to achieve higher accuracy and lower residual for model training. So that the model predicting the unseen data will have a higher chance to obtain the correct result. Of course, there is plenty of other powerful CNN available such as AlexNet, ResNet and more, those networks may also suitable applying in this data-set.

# Opinion
This Kaggle competition is challenging, because deep learning was totally new to me. I had to google numerous resources to gain intuition and understanding of how does deep learning work. Even though deep learning network is quite hard to master,it could solve the real world problems is exciting and motivating!

# Working enviroment
Google Colab
  - Keras 2.1.6
  - Python 3
  - Opencv 3.4.3
  - sklearn 0.19.2


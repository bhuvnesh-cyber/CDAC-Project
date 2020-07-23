# Plant-Seedlings-Classification
This project aimed at using deep learning model to classify the plant seedling by using a supervised learning technique Helping farmers in increasing productivity of crop and assisting in identifying the weed plants in initial stages by designing an intelligent model.

The data-set is available on Kaggle : (https://www.kaggle.com/c/plant-seedlings-classification/data).


## Data-set examination
### There are 12 species in the data-set which are shown below:
![xtrain_plant](https://user-images.githubusercontent.com/43289100/45993669-87d6f480-c0c2-11e8-86e7-cb5113af196b.png)

The data-set is split into two group, which are training and testing data.

## Apporach
* First understood how to leverage the power of data science to preprocess images.

* Second understood the plotting of distribution of images through matplotlib.

* Applied image processing on the images.

* converted images from RGB to HSV. It helps us distinguish certain colours and reduce other colors intensity on them.

* Apply closing opration(one of mophological opration where in important parts of HSV image will be extracted), segmentation and sharpening.

* Learned how to split data into training and testing set.

* Learn understand the theory and intuition behind convolutional neural networks and apply them to perform classification tests.

* Applied Data augumentation to prevent overfitting.

* Evaluate classification models and present results using confusion matrix and Plotting Loss value and Accuracy for each epoch.

## Pre-processing dataset
The training and testing images have been processed by using OpenCV libraries that extracted the plant seedling only and removed the background noise. The filtering process depending on the HSV values, retaining green HSV parameters and convert back to RGB format, which means only the green colour remains and the rest of the colour are removed.

Then the training and testing dataset have been normalized by dividing 255.0 to limit the pixel values within 0 to 1 and the labels are one-hot-encoded.

![BAR](https://user-images.githubusercontent.com/57914889/88261621-49251c00-cce4-11ea-894b-61aa7f925af9.PNG)

![CONFUSION](https://user-images.githubusercontent.com/57914889/88261624-4aeedf80-cce4-11ea-90b2-3268a7e65fcc.PNG)

![LOSS](https://user-images.githubusercontent.com/57914889/88261627-4b877600-cce4-11ea-8b20-24d0b19f21d1.PNG)

## Convolutional neural network (CNN)
CNN is a good choice while dealing with the image data. Designed CNN architecture based on personal experience, knowledge and, most important, the machine learning community and forum helps. The time spent a lot on tuning the model hyper-parameters in order to achieve higher accuracy and lower residual for model training. So that the model predicting the unseen data will have a higher chance to obtain the correct result. Of course, there is plenty of other powerful CNN available such as AlexNet, ResNet and more, those networks may also suitable applying in this data-set.

# Opinion
This Kaggle competition is challenging, because deep learning was totally a new concept. I had to google numerous resources to gain intuition and understanding of how does deep learning work. Even though deep learning network is quite hard to master,it could solve the real world problems which is exciting and motivating!

# Working enviroment
Google Colab
  - Keras 2.1.6
  - Python 3
  - Opencv 3.4.3
  - sklearn 0.19.2


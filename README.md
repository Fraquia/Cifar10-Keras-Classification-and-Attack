# Cifar10-Keras-Classification-and-Attack
Python Notebook where I trained and attacked a CNN on Cifar10 Dataset (15 Feb 2021)

## Project Description

### CNN Model

I've built a CNN using Keras Sequential to classify images in Cifar10 Dataset. In the model's architecure I used:

1. Conv2D
2. BatchNormalization
3. MaxPooling2D
4. Dense Layer
5. Dropout

To improve model's performances I also used Data Augmentation on the train set, using ImageDataGenerator from keras_preprocessing, trying to virtually increase the train set dimension, and reduce the gap from this one and ther real population I'm trying to classify.

Finally, I also used Google's GPU on training procedure to speed up execution time, that was like 35 times faster

### Attack 

To attack the model I refferred to Adversarial Robustness Toolbox. I attacked the model using: 

1. FGSM
2. JSMA

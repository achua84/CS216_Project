
# Project Overview

 In this project, we aim to gain insights about human visual acuity by applying these tests to machines. The main goal is to first train a convolutional-based neural network to recognize optotypes with low amounts of distortions so that it can use its knowledge to classify an unseen optotype from a testing set with optotypes with medium to high amounts of distortions. We used transfer learning, with the use of a VGG network, to obtain a baseline model for the problem. Then, we experimented with mixing the testing set with the training set, to determine if that could help the network make better predictions. My part of the project mainly involved the models with the mixed training/testing data. 


## Mixing_train_and_test.ipynb

In the first part of the notebook titled “Notebook Setup“, my partner, Brooke, wrote that code to read the images from the directories and divide them into training and testing sets. 

In the next section, I wrote code to take half of the testing set and include it into the training set. The next 25% of the testing set was put into the validation set and the remaining 25% was for the testing set. 

The next portion two portions involve hyperparameter tuning. In all experiments, both the VGG-16 and VGG-19 models were built with Tensorflow and Kera.

In the first portion, it was to see how many epochs was best to train both the VGG-16 and VGG-19 networks.

Then, the next portion experiments which how many layers should be frozen for both networks. 

After these experiments, the final model was trained and tested. 

Then, the learning curves for both the final data mixed model and the baseline model was graphed. 

After, I added some data visualization code to further explore the optotypes.  

Then, I used to model to display some of the images that the final model was able to predict correctly and incorrectly. 

## Baseline_model.ipynb

Even though Brooke took over this part, in the beginning, I was playing around with using the original dataset and the transfer learning models. The code in the notebook is a result of that. 

In the sections “Notebook Setup” and “Quick test to see how to use given code”, Brooke wrote all that code. I just ran it to see how it worked. 

The following sections was when I tried training the VGG-16 and VGG-19 networks with different number of epochs and different number of layers frozen (similar to the previous notebook). I also tried training the dataset with ResNet50, but training took longer than VGG-16 and produced similar results, so that was abandoned. 

I did not include the code Brooke implemented, as I did not contribute to her files. 



﻿﻿﻿[//]: # (Image References)
[image1]: ./results/Dataset_1.PNG
[image2]: ./results/Dataset_2.PNG﻿


#Semantic Segmentation Project
This is Project 2 of Udacity Self-Driving Car Nanodegree program Term3. 
In this project, the goal is to label the pixels of a road in images using a Fully Convolutional Network (FCN).
The project was created with the Udacity [Starter Code](https://github.com/udacity/CarND-Semantic-Segmentation).

## [Rubric](https://review.udacity.com/#!/rubrics/989/view) Points

## Content of this repo
 - `data` a directory with the  "Kitti Road dataset" for training the NN.
 - `runs` a Directory with test images
 - `main.py` - where the FCN is located 
 - `helper.py` - including helper functions and the VGG16 model
 - `project_test.py` - for testing the code
 - `README.md` Description of the Project by Udacity
 - `writeup.md` for submission of this Project
#####
## Result
#### Architecture

To label the pixels of a road in images a Fully Convolutional Network (FCN) was used. The Model is based on a trained VGG16 Model, with 1x1 convolutional layers, skip connections and upsampling for creating the FCN architecture. 
The convolutional layers and transpose convolutional layers include kernal reglatization and initilizaiton.








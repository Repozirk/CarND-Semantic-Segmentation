[//]: # (Image References)
[image1]: ./example/1.PNG
[image2]: ./example/2.PNG
[image3]: ./example/3.PNG
[image4]: ./example/2.PNG
[image5]: ./example/3.PNG


# Semantic Segmentation Project
This is Project 2 of Udacity Self-Driving Car Nanodegree program Term3. 
In this project, the goal is to label the pixels of a road in images using a Fully Convolutional Network (FCN).
The project was created with the Udacity [Starter Code](https://github.com/udacity/CarND-Semantic-Segmentation).

## [Rubric](https://review.udacity.com/#!/rubrics/989/view) Points

## Content of this repo
 - `data` a directory with the  "Kitti Road dataset" for training the NN.
 - `runs` a directory with test images
 - `example` a directory with example images
 - `main.py` - where the FCN is located 
 - `helper.py` - including helper functions and the VGG16 model
 - `project_test.py` - for testing the code
 - `README.md` Description of the Project by Udacity
 - `writeup.md` for submission of this Project
#####
## Result
#### Architecture
To label the pixels of a road in images a Fully Convolutional Network (FCN) was used. The Model is based on a trained VGG16 Model, with 1x1 convolutional layers, skip connections of the 3rd and 4th layer of the VGG16 Model and upsampling for creating the FCN architecture. 
The convolutional layers and transpose convolutional layers include kernel reglatization and initilization.

#### Optimmizer
Adam Optimizer was used for minimize the cross_entropy_loss 

#### Training
The FCN was trained one on an AWS p2.xlarge GPU instance with following parameters:
- `epochs = 10`
- `batch_size = 1`
- `keep_prob = 0.75`
- `learning_rate 0.0001`

With this hyper parameter, the loss drops below 0.1 within the first 2 epochs an achieves a final value of 0.0xx after 10 epochs

Example pictures of the FCN performance:
![alt text][image1] 
![alt text][image2] 
![alt text][image3] 
![alt text][image4] 
![alt text][image5] 











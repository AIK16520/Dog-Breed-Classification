# Dog-Breed-Classification
Step by step guide to make a dog breed classifier in python
Used Numpy, Pandas, Matplotlib, Tensorflow and Keras
Dataset from kaggle: https://www.kaggle.com/c/dog-breed-identification/data

Convert the Dog breed label to an array which has as much elements as the number of breeds
Each element is 0 except the true breed which is 1

First run the model on a 1000 image sample

Convert images to tensors
Group image to batches
Define and create the model: https://tfhub.dev/google/imagenet/mobilenet_v2_130_224/classification/5

Create 2 callbacks:
1: to keep track of the time 
2: to stop model early when accuracy isnt improving to save time

100 epoches declared

train model

use tensorboard to analyze the accuracy and loss
predict on validation data and output the breed with max probability
make a plot with image of the dog and the prediction output

Instead of just max prob we now output the top 10 prob with the true label highlighted in green

Make functions to save and load model

Now we train the full data and predictions on test data
Save the model trained on full data

load model trained on full data
perform the prediction on a custom image

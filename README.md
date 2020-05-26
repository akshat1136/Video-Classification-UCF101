# Video-Classification-UCF101
The repository contains video classification model for UCF101. 2D-LSTM network is used for this purpose. The processed dataset was taken from https://github.com/feichtenhofer/twostreamfusion. This was implemented in Google Colab. This is my first try on Sequence Model Implementation and I wanted to use them in vision task. Hence started working with videos. After reading few papers, I used the idea of using features of each frame in a sequence for learning and classification. 

The dataset used is already processed, each video sample is convered into sequence of frames and each sequence stored in separate folders. I have divided the code into 4 following parts:

1) DataInfo : Used this notebook to study about the details and structure of dataset and create useful info for further use.
2) DataFlow : Used to create a flow of data into the pipeline.
3) Model : The model is defined in this file using Tensorflow and Keras. Two parts of model creation are : Feature Extraction usinf Transfer Learning and Learning the pattern in sequence of features using LSTM.
4) Classification : The main file of the task, uses the previous data and features for classification of the sequence into 101 classes.

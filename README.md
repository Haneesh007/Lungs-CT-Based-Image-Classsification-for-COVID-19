# Lungs-CT-Based-Image-Classsification-for-COVID-19
-Performing Image Classification using Artificial Neural Networks

-Understand the working of Image Classification libraries and to evaluate the accuracy of the machine learning model

-Programming library used to analyse is Python 

-Technologies used will be Pandas, NumPy for the data handling part, Matplotlib for Data visualization part and TensorFlow (Keras, CNN model) for the Machine Learning Algorithms

-For this analysis the expectation is to achieve around 95% accuracy in classifying the images

-Understood working on Neural Networks

-Python we have TensorFlow library whose sub library Keras gives us the capabilities to create an artificial Neural Network and train the Neural Network

-The dataset we have used here is from GitHub

-It is an openly available dataset which contains images of CT of covid and non-covid patients

-We have in total 746 images There are in total 2 different types of CT images present in the dataset namely covid and non-covid

-The size of each image in the dataset varies and the input files are in PNG format

-Let us now proceed to understand the pre-processing part of the images

-We will initialize Image Data Generator which is present in the pre-processing library of TensorFlow’s Keras

-We will use these Image Data Generator to convert the input image dataset into features dataset using flow_from_directory() function

-In that function we will be passing our original dataset as input along with several parameters like target size, color mode, class mode, batch size, shuffle, zoom range, fill mode, subset, rotation range and so on.

-Let us now understand how we will be training our Neural Network using the training dataset prepared by Image Data Generator 

-We will be using Relu and Softmax as our activation function

-Activation function means how the weighted sum of the input is transformed to output from node or nodes of layers.

-First step for evaluation will be getting the predictions from the trained model, we will be using testing data set images for getting predictions from the trained Neural Network Classification model. 

-Next, we will be mapping the label from training images’ class indices to get the labels in the prediction dataset. 

-Then, finally we will be generating the accuracy score and other evaluation metrics of the model using the metrics library of Sci-kit learn. Accuracy score will be generated in percentage terms and will show us the percentage accuracy at which the Neural Network classification model is able to predict the output labels of the images in the testing data set. 

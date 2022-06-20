# Fashion-MNIST-Neural-Network
Using the python code to train several networks with different settings on this dataset. 
The Fashion MNIST dataset comprises 70,000 grayscale images of 10 fashion
products (tops, trousers, dresses, etc.). The data can be loaded straight from
Keras into a training set (60,000 images) and a testing set (10,000 images).
The images are 28*28 arrays with pixel values 0 to 255, and the labels are an
array of integersOur9, representing ten clothing classes. Predicting the clothing
class is the task here; it’s a multi-class classification task.
Before training Neural Network (NN) models, these images were first converted
into vectors to enable a fully connected network to classify the images by
applying the reshape function in Numpy. The vector values were rescaled
between 0 and 1. Also, a built-in function ‘to_categorical’ was utilised to convert
the integer labels (target labels, what we want to predict) to one-hot encoded
brands. 

Training a NN requires 4 steps:
● Build the architecture
● Compile the model
● Train the model
● Evaluate the model.

![image](https://user-images.githubusercontent.com/91108612/174505236-d0d374b5-8f46-4b2c-82e6-320603c03498.png)

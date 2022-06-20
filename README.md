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
1. Build the architecture
2. Compile the model
3. Train the model
4. Evaluate the model.

Exploring the evaluation of NN model:

1. Learning rates
![image](https://user-images.githubusercontent.com/91108612/174505236-d0d374b5-8f46-4b2c-82e6-320603c03498.png)

2. Different Optimizers
![image](https://user-images.githubusercontent.com/91108612/174505336-fdb09338-46e6-46ab-a79d-4499dc78c19a.png)

3. Different Batch Sizes
![image](https://user-images.githubusercontent.com/91108612/174505353-b4ff5134-09c3-4ae2-8542-42d50d9cec23.png)

4. different Architectures
![image](https://user-images.githubusercontent.com/91108612/174505399-d6adaba2-006a-4cc1-9030-c563666c5430.png)

Conclusion:

Neural Networks perform excellent on image classification. While building the
NN, many aspects need to be considered, like the architectures,
hyperparameters (learning rate, optimisers, batch sizes), as they could affect
the model performance. Optuna enables efficient hyperparameter tuning. It’s
notable that overfitting is easily diagnosed by monitoring the performance of
deep NN. In this task, it’s found that adjusting the batch size (32 or 64
recommended) and applying the Dropout method can address the over-fitting
issues. In terms of architecture, adding hidden layers will help improve the
model performance to some extent. CNN would generally be more powerful
than fully connecting ANN on image classification task. DeepCNN with Batch
Normalisation primarily performs the best with the highest accuracy 0.931 and
very low loss 0.278. Since this method can standardise the inputs to a layer for
each mini-batch, it can stabilise the learning rate by adding extra layers to the
deep neural network.

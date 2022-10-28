# Notes made while learning NPTEL DEEP Learning Course
## Important Notes
### Basics
- [ ] Large amounts of data
- [ ] Can be easily fooled
- [ ] They are also known as Black-Boxes
- [ ] Thus far has not been well integrated with prior knowledges
### TENSORFLOW
- Opensource
- Tensors in TF are multi dimensional arrays(DATA with higher dimensions)
- Operations which neural networks performs on tensors.
- PLatform flexibility
- It has auto differentiable capabilites
- Advanced support for threads , asynchronus computations.
# Prequisites
- Matrix
- Probability
- statistics
# Drawbacks
![image](https://user-images.githubusercontent.com/72144717/197602891-662d93a3-8880-414a-a8de-5f81394041ce.png)![image](https://user-images.githubusercontent.com/72144717/197610903-a2d78650-917f-47ff-a2c3-2964206cd20e.png)



# [Week 1](https://drive.google.com/drive/folders/13Coj35UfJ-Q5RQUcXikzdA2mUGLvEMDm)
## [Assignment link](https://onlinecourses.nptel.ac.in/noc22_cs124/unit?unit=17&assessment=181)
## Biological Neuron
![](https://miro.medium.com/max/1400/1*hkYlTODpjJgo32DoCOWN5w.png)


From Spring to Winter of AI, The Deep Revival, Faster, higher, stronger, Beating humans at their own games (literally), (Need for) Sanity, Motivation from Biological Neurons, McCulloch Pitts Neuron, Thresholding Logic, Perceptrons, Error and Error Surfaces, Perceptron Learning Algorithm, Proof of Convergence of Perceptron Learning Algorithm
## Perceptron
- Single layer cannot solve non-linear seprable data points.
![image](https://user-images.githubusercontent.com/72144717/198254671-14790d94-c6f6-486b-8731-e5f5ed8bd192.png)

 ![image](https://user-images.githubusercontent.com/72144717/197603446-387b3d4e-0082-4cf7-8c31-ebbf5b894a28.png)

![image](https://user-images.githubusercontent.com/72144717/197603760-76323edd-de27-44ad-a6ee-4d24df1ae6e9.png)

![image](https://user-images.githubusercontent.com/72144717/197604093-027792f6-bc6b-49d6-ac88-f42a1c31a073.png)

# [Week 2](https://drive.google.com/drive/folders/1XQtsxF1GHseEf-dJxyzSCXuwdXubhYAk)
## Sigmoid Neuron 
- [ ] Sigmoid is family of functions out of which we used logistic function


![image](https://user-images.githubusercontent.com/72144717/197604956-7dc81409-2f82-42fa-bbbe-1af7f78a7675.png)

![image](https://user-images.githubusercontent.com/72144717/197605237-501e13f6-9bea-479f-9aff-924e6ecab156.png)

![image](https://user-images.githubusercontent.com/72144717/197605510-3dea6104-3ffc-44b8-844d-60ad03d2fe4f.png)

![image](https://user-images.githubusercontent.com/72144717/197605581-11c3a43e-1fd3-46c4-a61f-97a390dfc604.png)



- [ ] For a perceptron there can be one or many extra inputs known as biases and weight is the slope of classifier line and biase allow us to shift line right or left.
- [ ] We guess weight `W` to minimize error called "Guess Work" then  we have Gradient descent and its variants an algorithm to do the same.
- [ ] If we set `W` to very High value we can recover the step function.



![image](https://user-images.githubusercontent.com/72144717/197610724-cf33582e-39bf-4814-bfe8-884fd692d709.png)

### Activating function 
Activation function decides whether a neuron should be activated or not by calculating  the weighted sum and further adding bias with it.It introduces non linerity . for eg.
- Unit or binary step
- Sigmoid logistic
- Tanh
- ReLU

- [ ] Now we should try approximating any different functions using neural networks
![image](https://user-images.githubusercontent.com/72144717/197617712-6a0644ae-ecc0-469e-a43d-00911d8e1c2f.png)

![image](https://user-images.githubusercontent.com/72144717/197616192-e44d1a30-1499-4c58-a81e-2b531405d832.png)

- [ ] We have understood for 1D input we require 2 neurons to create the tower after subtractint two different sigmoid fuunctions
- [ ] for 2D input we require 4 neurons
- [ ] Therefore, for nD input we require 2^n neurons


# [Week 3](https://drive.google.com/drive/folders/16FeJcuCzZi7iMLVf1pp0Qyym4ViEKLCF)
### Backtracking and variations of gradient Descent
used to find best W and B its goal is  to reach minimum error coordiantes.(Bottom of bowl)
#### Steps for using gradient descent algorithm
- [ ] Inititalize random weights and bias
- [ ] Pass an input through the network and get values from the output layer
- [ ] Calulate the error between the actual value and the predicted value
- [ ] Change respective value to reduce the error
- [ ] Repeat previous 3 steps until we minimize the error
#### Stochatic GD
#### mini batch GD (Most popular optimization algorithm)

### Cost function
![image](https://user-images.githubusercontent.com/72144717/198651428-d02ab1d6-86ac-4d97-be69-e7e5919905b5.png)

### Data Normalization
![image](https://user-images.githubusercontent.com/72144717/198267164-5521acaf-83db-4169-981e-68c44cdd2dbc.png)

### Weight Initialization 



### Multilayered Neurons(input,hidden,output layers)
- Deep neural networks are better than Shallow networks
- [Multilayered Neurons](https://youtu.be/AASR9rOzhhA)
![image](https://user-images.githubusercontent.com/72144717/197621318-d6ea4831-d98c-47b0-a6e5-00454cdf4d36.png)
## Backpropagation
## Feed forward neural networks
## Hyperparameters
- are the variables which determine the network structure

### Network parameters and training parameters


## Dropout
![image](https://user-images.githubusercontent.com/72144717/198268228-68382965-6cae-4a3b-9d1b-5d11aa6aa5b7.png)

## CNN (Convolutional neural network)
- Class of deep neural networks, most commonly used for analyzing visual imagery.
- Input is a multi-channeled image or a vector we say,

## RNN (Recurrent neural network)
- Backpropagation problems : vanishing gradient and Exploding gradient
- used for pattern recognition in handwritting

### LSTM 
- An RNN with feedback connections, they are capable of learning long term dependencies

~ Autoencoder /decoder



## Questions and Answers
![image](https://user-images.githubusercontent.com/72144717/198647394-3f9d9ccb-1ab1-44cc-a513-87b635c0e480.png)



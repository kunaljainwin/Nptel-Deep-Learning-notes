# [Notes made while learning NPTEL DEEP Learning Course] (https://onlinecourses.nptel.ac.in/noc22_cs124/)
## Important Notes
### Basics
- [ ] Large amounts of data
- [ ] Can be easily fooled
- [ ] They are also known as Black-Boxes
- [ ] Thus far has not been well integrated with prior knowledges
- [ ]  `VARIANCE` : Difference in performance of MLAlogo between Training and testing datasets
- [ ]  Ideal algorithm has low bias as well as low variance
- [ ]  https://youtu.be/wl1myxrtQHQ
### TENSORFLOW
- Opensource
- Tensors in TF are multi dimensional arrays(DATA with higher dimensions)
- Operations which neural networks performs on tensors.
- PLatform flexibility
- It has auto differentiable capabilites
- Advanced support for threads , asynchronus computations.
# Prequisites
- Matrix(Principle component analysis)
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
![image](https://user-images.githubusercontent.com/72144717/198653866-337fbf20-1bb3-41be-ab41-674379f40628.png)

- [ ] Now we should try approximating any different functions using neural networks
![image](https://user-images.githubusercontent.com/72144717/197617712-6a0644ae-ecc0-469e-a43d-00911d8e1c2f.png)

![image](https://user-images.githubusercontent.com/72144717/197616192-e44d1a30-1499-4c58-a81e-2b531405d832.png)

- [ ] We have understood for 1D input we require 2 neurons to create the tower after subtractint two different sigmoid fuunctions
- [ ] for 2D input we require 4 neurons
- [ ] Therefore, for nD input we require 2^n neurons


# [Week 3](https://drive.google.com/drive/folders/16FeJcuCzZi7iMLVf1pp0Qyym4ViEKLCF)
### Backtracking and variations of gradient Descent
used to find best W and B its goal is  to reach minimum error coordiantes.(Bottom of bowl)
![image](https://user-images.githubusercontent.com/72144717/198706119-407e95af-dbc3-4fa3-b80a-253c3d8d14d0.png)


#### Steps for using gradient descent algorithm
- [ ] Inititalize random weights and bias
- [ ] Pass an input through the network and get values from the output layer
- [ ] Calulate the error between the actual value and the predicted value
- [ ] Change respective value to reduce the error
- [ ] Repeat previous 3 steps until we minimize the error
#### Stochatic GD
#### mini batch GD (Most popular optimization algorithm)

### Cost function
- Average of mean squared errors
![image](https://user-images.githubusercontent.com/72144717/198651428-d02ab1d6-86ac-4d97-be69-e7e5919905b5.png)

### Data Normalization
![image](https://user-images.githubusercontent.com/72144717/198267164-5521acaf-83db-4169-981e-68c44cdd2dbc.png)

### Weight Initialization 
![image](https://user-images.githubusercontent.com/72144717/198700358-7b9e54c0-970c-4f92-8477-6b902e28a324.png)
- [ ] Its hard to predict which from linear regression and squiglly line will perform better on testing set
![image](https://user-images.githubusercontent.com/72144717/198700265-c7b217ac-5e65-4d67-894c-ca57da0d0765.png)
- [ ] This is called overfitting, i.e squiglly line is overfitting.


### Multilayered Neurons(input,hidden,output layers)
- Deep neural networks are better than Shallow networks
- [Multilayered Neurons](https://youtu.be/AASR9rOzhhA)
![image](https://user-images.githubusercontent.com/72144717/197621318-d6ea4831-d98c-47b0-a6e5-00454cdf4d36.png)
## Feed forward neural networks
## Backpropagation
### Information Content , Entropy and Cross Entropy
![image](https://user-images.githubusercontent.com/72144717/198691255-301a7e38-0447-49b6-9a2a-5758dd6b7ec3.png)

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


# [Week 4](https://drive.google.com/drive/folders/12FA_QRbs1Pjfx9WmKd-TOdk8uwKgLYda)
## Guess work (https://www.analyticsvidhya.com/blog/2021/06/guide-to-gradient-descent-and-its-variants-with-python-implementation/)
## Contour Maps+Comparison of all variations

![Alt] (https://firebasestorage.googleapis.com/v0/b/visitcounter-fef16.appspot.com/o/885513eee0b_33163162ddd94900b7d9f5b049e9b7e3_mv2.gif?alt=media&token=b71104a0-166d-4bd0-b297-6833f4485f4a)

Momentum based Gradient Descent
- Update rule
![image](https://user-images.githubusercontent.com/72144717/198705830-d1d37ffe-e45e-4426-991a-389ebd49611e.png)

Nesterov Accelerated Gradient Descent
![image](https://user-images.githubusercontent.com/72144717/198705944-57c9a1f9-e006-4638-a131-9af2fca669c3.png)

Stochastic And Mini-Batch Gradient Descent
![image](https://user-images.githubusercontent.com/72144717/198704959-98cf0054-b7ac-45a6-a4e3-7b31babe55f2.png)

Tips for Adjusting Learning Rate and Momentum

Line Search

Gradient Descent with Adaptive Learning Rate
![image](https://user-images.githubusercontent.com/72144717/198706245-17d81a34-be35-46ec-a822-3fcd10779728.png)

Bias Correction in Adam
![image](https://user-images.githubusercontent.com/72144717/198692228-7e90fedb-e987-4232-ba01-16a6899775fe.png)
#
![image](https://user-images.githubusercontent.com/72144717/198692291-6f5c6732-fd12-4e34-a180-d2fada93ea29.png)






#[Week 5]()
## Eigenvalues and Eigenvectors
[Nice video to understand](https://onlinecourses.nptel.ac.in/noc22_cs124/unit?unit=71&lesson=72)
[Proof about max eigenvalue of a row stochastic matrix](https://yutsumura.com/eigenvalues-of-a-stochastic-matrix-is-always-less-than-or-equal-to-1/)
- [ ]  It says that if the matrix is column stochastic matrix our Value of (Anot*Xnot)= M^n(Vector) becomes constant i.e k(LAMBDAd)(ed)

![image](https://user-images.githubusercontent.com/72144717/198712577-fafa638b-17a4-42bd-9e1e-ac3b709bdc0e.png)
![image](https://user-images.githubusercontent.com/72144717/198713752-ccc2db19-ff21-49ed-9cac-b371656b82e8.png)

[Orthonormal vectors are orthogonal/perpendicular vectors that are linearly independent and normal means that they are unit vectors](https://onlinecourses.nptel.ac.in/noc22_cs124/unit?unit=71&lesson=73)
[Helps](https://youtu.be/mdZVysybPrk?t=507)
Height in basketball 
[Helps](https://youtu.be/5eEPs8XS5AQ?t=367)
salary /Income tax corelation

- [ ] How do you prove linearly independent?
The linear independence of a set of vectors can be determined by calculating the determinant of a matrix with columns composed of the vectors in the set. If the determinant is equal to zero, then the set of vectors is linearly dependent. If the determinant is non-zero, then the set of vectors is linearly independent.08


#[Week 6]
## Autoencoders
[Helps](https://youtu.be/nTt_ajul8NY)
### Regularization 
Constraints the weights in a range
#### L1
![image](https://user-images.githubusercontent.com/72144717/198826812-e29c1d75-4471-4f68-a1f7-8ba1bb2ecc02.png)
constraints in squares
#### L2
![image](https://user-images.githubusercontent.com/72144717/198826851-64fcb6c9-e690-49f7-a3ee-42c79da5383f.png)
constraints in circles
#### Dropout


# [Week 7]
Evolution around 2006-2009
### problems with sigmoid
Sigmoid neuron : gradient vanishes if W is large , Axis is large(Not possible as we normalized)
- They are not 0 centered.
- ![image](https://user-images.githubusercontent.com/72144717/198829559-047158ce-30bc-4938-afc2-0afb98492ed5.png)

- [ ] People found tanh and ReLU good replacement for
![image](https://user-images.githubusercontent.com/72144717/198829585-8d392f28-14e0-4733-98c4-251746ec4de6.png)
## [ReLU](https://youtu.be/HxKaLyyGq50?t=1064)
ReLU -> Leaky ReLU -> Parameteric ReLU -> Exponential ReLU
![image](https://user-images.githubusercontent.com/72144717/198829631-f7d22edb-6dd9-4b63-84cd-430997b2939f.png)

![image](https://user-images.githubusercontent.com/72144717/198829006-2cfedd8d-002b-4aae-8b51-a3e95191d1e6.png)


# [Week 8]









## Questions and Answers
![image](https://user-images.githubusercontent.com/72144717/198647394-3f9d9ccb-1ab1-44cc-a513-87b635c0e480.png)
# 
![image](https://user-images.githubusercontent.com/72144717/198660971-ec1a1717-fb71-4dfa-a604-a8dba828c8c8.png)
#
![image](https://user-images.githubusercontent.com/72144717/198662678-addf7ab8-f028-49b5-aff2-6d470ec8e9fa.png)
#
![image](https://user-images.githubusercontent.com/72144717/198674039-0fcea958-845c-4874-8e29-5de54a1310ef.png)
#
![image](https://user-images.githubusercontent.com/72144717/198691489-296a9d69-653c-4c55-8197-502b41e3a44d.png)
#
![image](https://user-images.githubusercontent.com/72144717/198691668-987e7316-c12d-4f2f-831b-8666515bd3be.png)
#
![image](https://user-images.githubusercontent.com/72144717/198691916-9a12ec8a-0be1-4b80-a123-869fea457a0b.png)
#
![image](https://user-images.githubusercontent.com/72144717/198705272-d6ca2021-66c1-4cd0-8847-833fc7e0abc8.png)
#
![image](https://user-images.githubusercontent.com/72144717/198706432-a802cb50-a5d6-4f93-969e-acfc2a7294ed.png)
#
![image](https://user-images.githubusercontent.com/72144717/198706599-d6e8e601-8968-406e-95e2-06221e4977e9.png)
#
![image](https://user-images.githubusercontent.com/72144717/198706852-219d739c-f6d5-4a48-9886-07fa0ea879fc.png)
#
![image](https://user-images.githubusercontent.com/72144717/198706981-78f95ea9-f327-4330-b6f3-efd9c47251d5.png)
#
![image](https://user-images.githubusercontent.com/72144717/198707129-7fd63a83-5ce7-49e9-acfb-b407b40c1829.png)
#
![image](https://user-images.githubusercontent.com/72144717/198725157-2b21470c-0c4d-4f65-b368-1521b44277e9.png)
#
![image](https://user-images.githubusercontent.com/72144717/198727212-510f5dcc-2f83-4402-b61a-9ab0d05becbe.png)
#
Beause they are co-related
![image](https://user-images.githubusercontent.com/72144717/198727554-5454f847-583b-4a3a-87de-f1293b461723.png)
#
![image](https://user-images.githubusercontent.com/72144717/198823360-31193afa-8aa1-4534-8648-c397906c7717.png)
#
![image](https://user-images.githubusercontent.com/72144717/198827657-8d3c8b04-facb-443b-bb4d-3fce23d5a2a1.png)
#
![image](https://user-images.githubusercontent.com/72144717/198827744-e73c3be9-42c4-48c2-807d-d83284315b8c.png)
#
![image](https://user-images.githubusercontent.com/72144717/198830882-324f2347-2d2b-4715-b796-1545486a167b.png)
#
![image](https://user-images.githubusercontent.com/72144717/198830999-7e63896b-5dd6-4f44-84b3-58e8aa487753.png)
#
![image](https://user-images.githubusercontent.com/72144717/198831042-30be2817-5b52-4ffc-9e87-3379904cd434.png)
#
![image](https://user-images.githubusercontent.com/72144717/198831111-222442d2-05cc-4523-8727-e68b5e801197.png)
#
![image](https://user-images.githubusercontent.com/72144717/198831125-f86bbd05-fafd-4bf1-835b-0b47230e46e3.png)




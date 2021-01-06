# Deep Dive into Neural Networks

### Agenda

Discussion about ANN and it's components

Feedforward neural network

Loss function 

Gradient Descent and Backpropagation

Hyperparameter discussion

Write our first ANN



## Neural Network 

https://www.youtube.com/watch?v=aircAruvnKk&list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi

![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/46/Colored_neural_network.svg/280px-Colored_neural_network.svg.png)

This is the basic structure of a neural network

Each circle represents a node

Each arrow represents a connection called weights which gives an idea how strong the connection is

Input nodes pass the input data

So if a dataset has n input features it will have n input nodes

![](https://i.stack.imgur.com/X4y3f.png)

F1, F2, F3, F4, F5 -> F6

So in case of a dataframe like this we will have 3 input nodes

Output nodes represent the number of values a target node can take

So it it's a iris classification problem we can have 4 outputs since there are 4 categories of iris

In between the input and output nodes there can be any number of layers with nodes called hidden layers. 

Input nodes and output nodes are fixed but the number of hidden layers and hidden nodes is a hyperparameter.

**Weights and bias**

![](https://miro.medium.com/max/960/1*0lejoYyyQWjYzEP_BNW2nw.jpeg)

![](calc.png)

0.5 x 0.7 + 1.3 x -0.4 = -0.17 + 0.03 = -0.14

**Multi-layered neural network**

![](https://www.researchgate.net/profile/Facundo_Bre/publication/321259051/figure/fig1/AS:614329250496529@1523478915726/Artificial-neural-network-architecture-ANN-i-h-1-h-2-h-n-o.png)

**Activation Function**

Used to introduce non-linearity  

y = x1^2 + x2^3

![](https://miro.medium.com/max/1200/1*ZafDv3VUm60Eh10OeJu1vw.png)

Activation function does two things :-

1. Add non-linearity
2. Lights up or kills a neuron

**Softmax function**

![](https://deepnotes.io/public/images/softmax.png)

![](https://i2.wp.com/sefiks.com/wp-content/uploads/2017/11/softmax1.png)

S(2) = e^2/(e^2+e^1+e^0.1)

S(1) = e^1/(e^2+e^1+e^0.1)

S(0.1) = e^0.1/(e^2+e^1+e^0.1)

S(2) + S(1) + S(0.1) = 1

Linear -> MSE

Logistic -> Cross-Entropy

**Cross-entropy loss**

![](https://image.slidesharecdn.com/d3l1lossfunctions-181009074432/95/loss-functions-for-deep-learning-javier-ruiz-hidalgo-upc-barcelona-2018-32-638.jpg?cb=1539071280)

L = - ((0 * log(0.1)) + (1 * log(0.7) + (0 * log(0.2)))

Why cross-entropy and not mean square loss

**Gradient Descent**

Neural network does forward propagation to give a certain output

We then see how much the output differs from expect output using the cost/loss function

Our goal is to reduce the loss function and get the global minima using the weights and biases

To do this start with random set of weights and gradually nudge them to reach the local minima

![](https://miro.medium.com/max/1458/1*E-5K5rHxCRTPrSWF60XLWw.gif)

![](https://qph.fs.quoracdn.net/main-qimg-ba2f4cd540b8f2b5570976afd247b65d)

![](https://cdn-images-1.medium.com/max/1600/0*fU8XFt-NCMZGAWND.)



https://www.youtube.com/watch?v=IHZwWFHWa-w&list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi&index=2

![](https://i.stack.imgur.com/pYVzl.png)

**Backpropagation**

![](1.png)

The output here vastly differs from expected

![](2.png)

This is the output we want

To achieve this we need to push up the activation at 2 to 1 and push the rest down to 0

![](3.png)

3 ways to change to output

1. Change bias
2. Change weights
3. Change activations

![](4.png)

![](5.png)

Cumulative sum of changes. Recursively apply the process and move backwards and hence backpropagation

![](https://thumbs.gfycat.com/FickleHorribleBlackfootedferret-small.gif)

https://www.youtube.com/watch?v=Ilg3gGewQ5U&list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi&index=3

### Training concepts

**Batch**

Batch is a set of data points

![](https://suniljangirblog.files.wordpress.com/2018/12/descent.png?w=908)

**Learning rate**

Pace at which you would want to train

![](https://www.jeremyjordan.me/content/images/2018/02/Screen-Shot-2018-02-24-at-11.47.09-AM.png)

**Batch size and epoch**

Batch size is number of data points present in a single training step i.e iteration

An epoch is when all the examples in the training dataset is visited once



Difference between neural networks and other things you saw until now

Neural networks global minima might look like below, so you need to train more to reach global minima

If batch gd is used can get stuck in local minima hence mini batch gd is used

![](https://i.stack.imgur.com/rPx0Q.png)

**Underfitting and overfitting**

![](https://miro.medium.com/max/1125/1*_7OPgojau8hkiPUiHoGK_w.png)

Underfitting is battled by increasing the capacity of network

Overfitting is battled by adding regularisation techniques



**Input normalization**

Keep pixel values between 0-1

Divide every pixel value by 255

**Training and Test dataset**

We divide the dataset into train and test to validate if the model is not overfitting

### Dropout

**Dropout** is a regularisation technique which can be used to reduce overfitting

You can imagine Dropout as training multiple neural networks to do a task popularly called ensemble technique

Used to remove dependency on particular neurons

At test time all the neurons are used but the output is multiplied by a factor so as not to overwhelm

![](https://miro.medium.com/max/1044/1*iWQzxhVlvadk6VAJjsgXgg.png)

![](https://s3-ap-south-1.amazonaws.com/av-blog-media/wp-content/uploads/2018/04/1IrdJ5PghD9YoOyVAQ73MJw.gif)



![](https://media.makeameme.org/created/enough-blah-blah.jpg)
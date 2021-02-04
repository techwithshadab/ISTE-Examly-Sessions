# Intro to Deep Learning 

### Background

![](https://i.makeagif.com/media/10-14-2015/w1w5Aq.gif)

**Why now ?**

**How now ?**

![](https://miro.medium.com/max/3200/1*HFD6SjpXIamKzw4O4HmuMQ.jpeg)

### Objectives

Learn the theory, background and intuitions of a neural network

To be able to train a neural network to achieve industrial quality results

Be industry ready for a deep learning position



Few classes of intense content

Need collaborative effort from each other

Post on Linkedin, medium



**Today we shall write a small piece of content about anything you learned from class today on Linkedin**



Quiz after session

### What we will be learning

1. What is Deep Learning and how is it different from machine learning
2. Theory of neural networks
3. Writing your first neural network
4. More complex neural networks
5. Training a neural network to reach industrial quality results on a popular dataset
6. Apply deep learning for NLP



### Some myths

Machine learning is not prerequisite for Deep Learning

Maths is compulsory for deep learning(Intuition is)

Need to do a lot of certifications online to be good at ML/DL

Need 1-2 years of preparation to be good at deep learning

Not possible for changing career paths in between

### What is machine learning

![](https://miro.medium.com/max/700/1*Yi64yzIRh5iH3p2Blh8GvA.jpeg)





![](https://cdn.hashnode.com/res/hashnode/image/upload/v1586981100950/M50u6HA1K.png?auto=format&q=60)

![](https://storage.ning.com/topology/rest/1.0/file/get/2808354979?profile=original)

![Types of ML](https://miro.medium.com/max/1200/1*9Eu_-DDMZ_bP_t94_MMEYA.png)

# Supervised Learning

### Classification

![](https://i.ytimg.com/vi/rz-TFeeo7w0/maxresdefault.jpg)

![](https://miro.medium.com/max/2844/1*hCxU4nK6ulpnwhSpgWiPPg.png)



### What is Deep Learning

**Deep learning** (also known as **deep structured learning**) is part of a broader family of [machine learning](https://en.wikipedia.org/wiki/Machine_learning) methods based on [artificial neural networks](https://en.wikipedia.org/wiki/Artificial_neural_networks) with [representation learning](https://en.wikipedia.org/wiki/Representation_learning). Learning can be [supervised](https://en.wikipedia.org/wiki/Supervised_learning), [semi-supervised](https://en.wikipedia.org/wiki/Semi-supervised_learning) or [unsupervised](https://en.wikipedia.org/wiki/Unsupervised_learning).

![](https://i.imgflip.com/41wp8h.jpg)

Deep Learning uses neural networks to solve the same tasks as machine learning

# Machine Learning vs Deep Learning

![](https://busyteacher.org/uploads/posts/2019-09/1569775072_screen-shot-2019-09-29-at-12.37.27-pm.png)

Multiple ways to solve the same problem

![](<http://www.videantis.com/wp-content/uploads/2018/07/LSVRC-winners-over-time.png>)

![ML vs DL](https://qph.fs.quoracdn.net/main-qimg-6c1dc5666bd31bf16120d332957b4059)



### Applications of Deep Learning

https://www.youtube.com/watch?v=gLoI9hAX9dw

Dog vs cat classfier

**Object Detection**

![](<https://miro.medium.com/max/503/1*xWntyXM0W-SuDMgWMM6mCg.png>)

Like mask detection

**Image Segmentation**

![](<https://s3-ap-south-1.amazonaws.com/av-blog-media/wp-content/uploads/2019/03/Screenshot-from-2019-03-28-11-45-55.png>)

**Face detection**

![](<https://cdn2.hubspot.net/hubfs/3873528/FACIAL-RECOGNITION-compressor.png>)

**Prisma like apps**

![](<https://forums.fast.ai/uploads/default/original/3X/c/f/cf5bc18c3b8a3761e341056c3f131012001d4248.jpeg>)

**Generative networks**

![](<https://www.lyrn.ai/wp-content/uploads/2018/12/Faces-example-1366x877.jpg>)

![](https://miro.medium.com/max/3116/1*aRZSwFlnodTH3FbP70yNXg.png)

**Speech Recognition**

![](https://miro.medium.com/max/2600/1*gosRRsHwIkGH-Hr1rt6Z0g.jpeg)



## Neural Network and biological intuitions

![](https://miro.medium.com/max/1220/1*SJPacPhP4KDEB1AdhOFy_Q.png) 

**Basic components**

Neurons/Nodes

Weights

![](1.png)

![](2.png)

![](3.png)

![](4.png)



**What is an image ?**

Image is nothing but a matrix

Black and white image is a 2d matrix

RGB image is a 3d matrix

[1 3  6

9 2   9

0 34 89] -> [1 3 6 9 2 9 0 34 89]

300x300 -> 90000



![](5.png)

![](6.png)

Higher value of the number means higher the activation

![](8.png)

![](9.png)

![](10.png)

![](12.png)



**Artificial Neural Network**

![](https://www.researchgate.net/profile/Facundo_Bre/publication/321259051/figure/fig1/AS:614329250496529@1523478915726/Artificial-neural-network-architecture-ANN-i-h-1-h-2-h-n-o.png)



Hierarchy :-

1. Input layer -> Determined by size of input
2. Hidden layers -> Hyperparameter to be tuned
3. Output layer -> Defined by target 
## Agenda

CNN components discussion

Regularization techniques discussion

Intro to CNN architectures



### 1x1 Convolution

In neural networks 1x1 convolutions are generally used to reduce the dimensions of input in the filter dimension. As the depth of the neural network is increased in general the filter dimension is increased which leads to a lot of computation. To save this effort 1x1 convolutions are used. They were extensively used in Google's inception architecture

![](https://raw.githubusercontent.com/iamaaditya/iamaaditya.github.io/master/images/conv_arithmetic/full_padding_no_strides_transposed_small.gif)

Used to mix and match channels

# Global Average Pooling

**Average Pooling** :-

[![img](https://camo.githubusercontent.com/f8a3d9e7b98940d0621263304047dbf8fbeb3e50/68747470733a2f2f656d626172632e6f72672f656d626172635f6d6c692f646f632f6275696c642f68746d6c2f5f696d616765732f696d6167653130392e706e67)](https://camo.githubusercontent.com/f8a3d9e7b98940d0621263304047dbf8fbeb3e50/68747470733a2f2f656d626172632e6f72672f656d626172635f6d6c692f646f632f6275696c642f68746d6c2f5f696d616765732f696d6167653130392e706e67)

Max pooling preferred over average pooling

**Why we need pooling**

1. To reduce the input size
2. To achieve local translation and rotation invariance

Average pooling with size equal to that of kernel to constrain it to a single value per channel. Generally used at the output layer in fully convolutional networks

[![img](https://camo.githubusercontent.com/0cba6eeb4478e3cb08ce22755cb0c08ce9ea8a1f/68747470733a2f2f70656c746172696f6e2e636f6d2f7374617469632f676c6f62616c5f617665726167655f706f6f6c696e675f612e706e67)](https://camo.githubusercontent.com/0cba6eeb4478e3cb08ce22755cb0c08ce9ea8a1f/68747470733a2f2f70656c746172696f6e2e636f6d2f7374617469632f676c6f62616c5f617665726167655f706f6f6c696e675f612e706e67)

Added to replace fully connected neural networks

# Receptive Field

The amount of the image the network looks at. It increases as the depth of the network increases

## Regularization techniques

### Batch Normalization

Used to normalize the input to every layer

![](https://miro.medium.com/max/810/1*Hiq-rLFGDpESpr8QNsJ1jg.png)

### Dropout

Regularization technique to improve the capability of a network by giving the power of an ensemble of networks

![](https://qph.fs.quoracdn.net/main-qimg-94a1d5e149ab864bfa20ef7e5242777d.webp)

### Image Augmentation



![](https://raw.githubusercontent.com/aleju/imgaug-doc/master/readme_images/small_overview/noop_image.jpg)

![](https://raw.githubusercontent.com/aleju/imgaug-doc/master/readme_images/examples_grid.jpg)



#### L1 and L2 regularization

![](https://miro.medium.com/max/2546/1*zMLv7EHYtjfr94JOBzjqTA.png)

####  Label Smoothing

Have soft labels instead of hard labels

Dog Cat Horse

0.9  0.05 0.05

0.05 0.9  0.05

![](https://image.slidesharecdn.com/aimeetgans-170110113744/95/generative-adversarial-networks-and-their-applications-39-638.jpg)


# Implementation of Resnet50 with Pytorch and TorchFusion
---
Resnet50 implementation of the paper [Deep Residual Learning for Image Recognition](https://arxiv.org/abs/1512.03385) in Pytorch and TorchFusion
# Architecture
---
Resnet(Residual Network) is a kind of deep learning architecture which makes use of residual units which helps to overcome the varnishing gradient problem that affects deep neural networks. According to the paper:
> The resnet consist of residual units which is made by adding the input of the previous layer to the output of the next layer. The first convolutional layer the residual network has a kernel size of seven, stride of 1 and a padding of 3. The output of this first convolutional layer is then passed to the first residual block. The first residual block is made up three residual units, and the size of it's input feature map of the first residual unit is equal to the size of the output feature map of the last residual unit in the first block. The next three residual blocks are consist of 4, 6, 3 residual units respective with there output feature maps of there last residual units equal half the input feature map of the first residual unit the each block. The output from the last residual block is passed to a maxpooling layer then the globalaveragepool the of the new output is computed then passed to the fully connected layer.

Residual Networks prevents issues such as: <br>
1.) Vanishing Gradients: For very deep networks the computed gradients at times get so small i.e very close to zero that the cannot propagate through the network hence they are said to varnish. <br>
2.) optimization difficulty: The model parameters tends to increase as the number of parameters increases, this make it more difficult for the model to train an also lead to higher training error.


# Requirements
---
* Pytorch
* TorchFusion
* numpy
* PIL
* matplotlib
* Python

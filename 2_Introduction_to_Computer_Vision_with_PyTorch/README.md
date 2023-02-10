# README

- 这是微软的pytorch vision，里面其实只用微软的学习课程中下载的，微软也搞了一个类似colab的沙盒，不过比起colab各种方面无疑差了很多，不过对于中国玩家而言可能比较友好了（colab被墙）

## **注意事项**

#### wget

- `wget`属于linux的命令，windows下没有，所以可以从github中直接下载下来（去搜索相应的路径即可，不过这里的文档都已经有相应的文件了）
- 如果一定需要安装`wget`，可以在[这里](https://eternallybored.org/misc/wget/)下载，下载后解压，然后将解压后的文件夹放到`C:\Windows\System32`下，然后在`cmd`中输入`wget`，如果出现了`wget`的帮助信息，那么就说明安装成功了
- 这些文档放在colab中都可以直接运行（装好相应的依赖之后）

#### use GPU

- 如果想要使用GPU(由于自己的本地计算机没有nvidia显卡，所以直接把对应的ipynb放在colab上面跑了，对应训练好的ipynb和数据都放在`testOnColab`文件夹下，起初是想用`paddlepaddle`来训练的可是百度的平台不支持pytorch)
- 可以在Colab的`Runtime`中选择`Change runtime type`，然后在`Hardware accelerator`中选择`GPU`，然后点击`Save`，然后重新运行代码即可，一般会分配到`Tesla T4`

> 比如`6-TransferLearning.ipynb`的代码放在本地用十六核的CPU跑可能需要两小时以上，放在colab上面用GPU跑只需要几分钟就好了。

#### Pytorch版本

在第一个笔记本到第六个笔记本中，使用的版本如下：

```python
print(torch.__version__) # 1.11.0+cpu
print(torchvision.__version__) # 0.12.0+cpu
```

而实际要求的版本如下：

```
torchvision==0.13.0
torch==1.12.0
```

#### 预训练模型参数下载

自己在运行的时候首先由于在本地也训练了一次，参数放在`./torch/models`文件夹下，由于参数太大就不上传github了。



# Introduction to Computer Vision with PyTorch

- 53 min
- Module
- 8 Units

Machine Learning

We'll learn about different computer vision tasks and focus on image classification, learning how to use neural networks to classify handwritten digits, as well as some real-world images, such as photographs of cats and dogs. We'll be using one of the most popular deep learning frameworks, PyTorch!

## Learning objectives

In this module you will:

- Learn about computer vision tasks most commonly solved with neural networks
- Understand how Convolutional Neural Networks (CNNs) work
- Train a neural network to recognize handwritten digits and classify cats and dogs.
- Learn how to use Transfer Learning to solve real-world classification problems with PyTorch

Add

## Prerequisites

- Basic knowledge of Python and Jupyter Notebooks
- Familiarity with PyTorch framework, including tensors, basics of back propagation and building models
- Understanding machine learning concepts, such as classification, train/test dataset, accuracy, etc.

## This module is part of these learning paths

- [PyTorch Fundamentals](https://learn.microsoft.com/training/paths/pytorch-fundamentals/)

- [Introduction](https://learn.microsoft.com/en-us/training/modules/intro-computer-vision-pytorch/1-introduction)2 min
- [Introduction to processing image data](https://learn.microsoft.com/en-us/training/modules/intro-computer-vision-pytorch/2-image-data)5 min
- [Training a simple dense neural network](https://learn.microsoft.com/en-us/training/modules/intro-computer-vision-pytorch/3-train-dense-neural-networks)10 min
- [Use a convolutional neural network](https://learn.microsoft.com/en-us/training/modules/intro-computer-vision-pytorch/4-convolutional-networks)10 min
- [Train multi-layer convolutional neural network](https://learn.microsoft.com/en-us/training/modules/intro-computer-vision-pytorch/5-multilayer-convolutions)10 min
- [Use a pre-trained network with transfer learning](https://learn.microsoft.com/en-us/training/modules/intro-computer-vision-pytorch/6-transfer-learning)10 min
- [Solving vision problems with MobileNet](https://learn.microsoft.com/en-us/training/modules/intro-computer-vision-pytorch/7-mobilenet)5 min
- [Summary](https://learn.microsoft.com/en-us/training/modules/intro-computer-vision-pytorch/8-summary)1 min

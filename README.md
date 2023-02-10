# README

记录一下自己在学习微软家pytorch教程的笔记和保存的`ipynb`文件，[Microsoft Learn](https://docs.microsoft.com/learn/paths/pytorch-fundamentals/)的东西感觉在他们自己的沙盒上运行的实在太慢了，体验不是怎么好，自己放在本地和colab笔记本上又重新跑了一遍，大概是对四个模块的认识更深一点了。

```
\pytorch_funfamentals


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----          2023/2/5      9:37                1_Introduction_to_PyTorch
d-----         2023/2/11      7:11                2_Introduction_to_Computer_Vision_with_PyTorch
d-----          2023/2/9     16:19                3_Introduction_to_Natural_Language_Processing_with_PyTorch
d-----         2023/2/10     13:06                4_Introduction_to_audio_classification_with_PyTorch
-a----         2023/2/11      7:11             12 README.md
```

- 模块一主要用一个案例来教会你tensors、autograd、optimization这些技巧，整个文件夹用cpu跑也是完全没问题的
- 模块二则介绍了各种cv的net还有transfer-learning等等概念，模型参数大起来了用cpu跑就很慢，所以底下多创建了一个文件夹`testOnColab`里面的文件是在colab上用`Tesla T4`跑过的(每次都是分配到T4)
- 模块三则介绍了rnn、lstm、生成文本的一些内容，不过没有讲transformer和bert了，在之前的版本应该是有的（这里自己去github上下载了也放在这里）。
- 模块四介绍了将waveform转化成spectrograms再导出png图片，最后通过cnn对图片训练达到yes和no语音分类的效果。


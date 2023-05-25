+++
author = "Rico0807"
title = "U-Net家族发展史"
date = "2023-05-25"
description = "本篇博客主要介绍U-Net家族发展史"
tags = [
	"U-Net",
]
series = ["Themes Guide"]
aliases = ["migrate-from-jekyl"]


+++

## U-Net 家族发展史

<font color="#00aa00" size = "5">**2015**</font> 

* U-Net: Convolutional Networks for Biomedical Image Segmentation (MICCAI)	[paper](https://arxiv.org/pdf/1505.04597.pdf)

![](U-Net-Original.jpg)

​	本文首次提出由编码路径和解码路径组成的U型结构网络，U-Net。其中，编码路径由“卷积核+激活层+池化层”组成，解码路径由“卷积层+激活层+上采样层”组成。该U型网络结构中，编码路径和解码路径通过 Skip Connection连接，以保证浅层网络中的语义信息不会丢失。
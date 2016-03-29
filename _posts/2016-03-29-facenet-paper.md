---
title:"论文笔记—FaceNet:A Unified Embedding for Face Recognition and Clustering
---

## Introduction

[FaceNet](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&ved=0ahUKEwjp7ubb9uXLAhUM5mMKHSaxCqAQFggjMAA&url=http%3A%2F%2Farxiv.org%2Fabs%2F1503.03832&usg=AFQjCNGc_8hK46EzkvB0FOZ4eqObLhD53Q&sig2=xRIbjMEzMIjKLkEFWLdgFQ&cad=rjt) 是google提出的一个用于脸部识别及其他功能的模型。

## Background

传统的人脸识别方法利用siamese网络来提取人脸特征，再用SVM等方法进行分类。作者言：

> *implementing face verificationand recognition efficiently at scale presents serious challengesto current approaches*.

## Achievement

* 提出FaceNet模型，将图像特征映射到欧式空间的向量上。图像特征向量的距离可以表示图像的相似程度。
* 使用深度卷积网络直接对Embedding Function进行优化，而不优化*intermediate* *bottleneck* *layer*。
* 使用<mark>Triplet</mark> <mark>Loss</mark>

## Details

1. 为什么可以直接优化 Embedding Function
2. 何为intermediate bottleneck layer
3. Triplet中的正负样本是如何选取的


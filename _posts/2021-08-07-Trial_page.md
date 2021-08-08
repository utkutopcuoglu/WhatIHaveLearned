---
title: "Why Convolutions?"
description: "Why do we use Convolutions in CNN"
layout: post
toc: false
comments: true
# image: images/some_folder/your_image.png
hide: false # hide from homepage
search_exclude: true # set the front matter search_exclude to false if you don't want users to find your hidden post in a search.
categories: [fastpages, jupyter] # Add tags to table of content
# You can toggle the display of tags on/off by setting show_tags to true or false in _config.yml:
# Set this to true to display tags on each post
# show_tags: true
metadata_key1: metadata_value1
metadata_key2: metadata_value2
---

# Brief
Convolutional Neural Networks are special type of networks which are used widely in computer vision (tasks like object detection, tracking, segmentation etc.). It imitates the visual cortex and is a very important field in deep learning (since there are plenty of image data for these data hungry models.).

I will briefly explain a simple CNN architecture and important functions in between.

A simple CNN architecture includes the **convolution**, **activation function**, **pooling**, **flattening** operations which might be then connected to a regular neural network (**dense layer**) with a **softmax** classifier (for normal classification) or multiple **sigmoid** outputs (for multi-class classificaton).

In this post I will only focus on why convolution is useful.

### Why Convolutions?
Regular neural networks can learn from pixels also, but it will use all pixels as inputs and meanwhile might overfit to the noise in the image. This way a regular NN needs many more images to learn the relations between pixels and much it will have much more parameters to learn. But we can make it easier for it learn by focusing on the probably most important information in an image.

To human eye, a single pixel has no value, but a group of pixels can form a shape (eye, cat, etc.). Especially close pixels can carry more meaningful spatial information. This means if we focus on regions, rather than single pixels, we might even be able to avoid looking to the whole picture -> hence we will have less features (pixels) to care about and less parameters -> this way we can learn faster in a more efficient way.

This is what the convolution operation does. It looks at a region in an image and adds a non-linearity function (activation function) just like a regular neural network. This way the relation between pixels can be understood with much less parameters and processing. This is also called **Sparsity of Connections**. Another advantage, the information we learn by looking at small regions share many features (like edges, corners) which can be generalized across the image and re-used for many regions over the image. Being able to re-use the same convolution operation (or filter) is called **Parameter Sharing** and it also reduces the parameters in CNN (that has to be learned.).

To summarize, the **Sparsity of Connections** and **Parameter Sharing** makes the convolution operation particularly useful in CNNs.

---
toc: false
layout: post
categories: ["Deep Learning", "NLP"]
title: Recurrent Neural Networks
description: "Traditional Neural networks found it very difficult to execute tasks in Natural Language Processing (NLP). To understand a sentence it is important to both understand each word, it's relationship with the previous and successive words and also the context in which the word is being used. Recurrent Neural Networks adopt a structure that helps solve this issue and is the main focus of this article."  
hide: true
---
A recurrent neural network (RNN) is a type of Neural Network that allows previous outputs to be used as inputs while using hidden states. It is called a Recurrent Network because it repeatedly takes an input, uses it to modify a hidden layer and then provides an output which is then fed back to the hidden layer along with the next input. The hidden layer acts as "memory" that keeps track of the previous inputs by how the weights in the layer were modified by the said input. Consider an example of a RNN working on predicting the next word in a sentence. The first word is passed into a hidden layer, the output of this hidden layer along with the next input is then passed on to the next hidden layer and this process continues till all the inputs are passed on to the final output layer which predicts the final word. In this way, the RNN has an "understanding" of each word in the network and can make a reasonable prediction of the final word.


# TODO: Add image of RNN for predicting the next word here::

The structure used here is a many-to-one type of RNN. Many other RNN architectures have been developed to accomplish other tasks like music generation, sentiment analysis and machine translation. 




---
toc: true
layout: post
description: A quick review of the Jargon before proceeding through the lessons
categories: [markdown]
title: Jargon Review
---

#Chapter 1: Introduction

1. Do you need these for deep learning?

   - Lots of math T / F: **False**, a lot of libraries have been created to take care of the complex math parts and allow us to focus on training models
   - Lots of data T / F: **False**, a lot of great results have been seen with small amounts of data
   - Lots of expensive computers T / F: **False**, there are a lot of free and cheap options avaliable to create and deploy deep learning models
   - A PhD T / F: **False**
   
1. Name five areas where deep learning is now the best in the world.
    - Image Recognition
    - Natural Language Processing
    - Recommendation Systems
    - Playing games like chess, Go etc.
    - Image generation
1. What was the name of the first device that was based on the principle of the artificial neuron?
    - The Perceptron
1. Based on the book of the same name, what are the requirements for parallel distributed processing (PDP)?
    - Processing Units 
    - State of Activation
    - Output Function
    - Pattern of connectivity
    - Propagation Rule
    - Activation Rule
    - Learning rule
    - Environment.
1. What were the two theoretical misunderstandings that held back the field of neural networks?
    - Cannot learn simple functions like XOR
    - Require a lot of computational power and was very slow.
1. What is a GPU?
    - Graphical Processing Unit. Specialized CPU working at a faster speed.
1. Why is it hard to use a traditional computer program to recognize images in a photo?
    - It is very complex to create a logic for reading in the pixels and performing a method of recognition, because we ourselves can't write these steps down. These happen automatically in our brains without us being conscious about it.
1. What did Samuel mean by "weight assignment"?
    - By weight assignment, Arthur Samuel means to assign a particular set of values to the different variables(weights) involved in the program. The inputs and weights are the two different values involved in a program.
1. What term do we normally use in deep learning for what Samuel called "weights"?
    - They are also called parameters
1. Draw a picture that summarizes Samuel's view of a machine learning model.
![]({{ site.baseurl }}/images/ArthurSamuelModel.png "Arthur Samuel's Model")
1. Why is it hard to understand why a deep learning model makes a particular prediction?
    - 
1. What is the name of the theorem that shows that a neural network can solve any mathematical problem to any level of accuracy?
    - Universal approximation theorem
1. What do you need in order to train a model?
    - Data, a set of weights and 
1. How could a feedback loop impact the rollout of a predictive policing model?
    - This model will predict where more arrests will be made. If there is a bias in the data collection, the model will predict those areas where previous arrests had been high. After seeing these results, the police departments may assign more policemen to patrol areas which have a high probability of arrests which may cause even more arrests being made.
1. What is the difference between classification and regression?
    - Classification involves predicting discrete classes which the elements belong into and regression involves predicting a continuous variable for a given set of independent variables.
1. What is a validation set? What is a test set? Why do we need them?
1. What will fastai do if you don't provide a validation set?
    - Automatically create a validation set with 20% of the training data.
1. Can we always use a random sample for a validation set? Why or why not?
1. What is overfitting? Provide an example.
    - Predicting the variables so that the 
1. What is a metric? How does it differ from "loss"?
1. How can pretrained models help?
    - Pretrained models can help in reducing the time taken for training and 
1. What is the "head" of a model?
1. What kinds of features do the early layers of a CNN find? How about the later layers?
1. Are image models only useful for photos?
    - No, sounds have been transformed to images based on their frequencies/loudness and then passed on to image models to identify the type of sound.
1. What is an "architecture"?
    - Architecture refers to the structure of the neural network in terms of the inputs it takes, the number of hidden layers and the number of outputs of each layer/
1. What is segmentation?
1. What is `y_range` used for? When do we need it?
    - `y_range` is a paremeter that defines the range of values the prediction can take. It is used to 
1. What are "hyperparameters"?
1. What's the best way to avoid failures when using AI in an organization?

---

# Production:

1. Provide an example of where the bear classification model might work poorly in production, due to structural or style differences in the training data.
1. Where do text models currently have a major deficiency?
1. What are possible negative societal implications of text generation models?
1. In situations where a model might make mistakes, and those mistakes could be harmful, what is a good alternative to automating a process?
1. What kind of tabular data is deep learning particularly good at?
1. What's a key downside of directly using a deep learning model for recommendation systems?
1. What are the steps of the Drivetrain Approach?
1. How do the steps of the Drivetrain Approach map to a recommendation system?
1. Create an image recognition model using data you curate, and deploy it on the web.
1. What is `DataLoaders`?
1. What four things do we need to tell fastai to create `DataLoaders`?
1. What does the `splitter` parameter to `DataBlock` do?
1. How do we ensure a random split always gives the same validation set?
1. What letters are often used to signify the independent and dependent variables?
1. What's the difference between the crop, pad, and squish resize approaches? When might you choose one over the others?
1. What is data augmentation? Why is it needed?
1. What is the difference between `item_tfms` and `batch_tfms`?
1. What is a confusion matrix?
1. What does `export` save?
1. What is it called when we use a model for getting predictions, instead of training?
1. What are IPython widgets?
1. When might you want to use CPU for deployment? When might GPU be better?
1. What are the downsides of deploying your app to a server, instead of to a client (or edge) device such as a phone or PC?
1. What are three examples of problems that could occur when rolling out a bear warning system in practice?
1. What is "out-of-domain data"?
1. What is "domain shift"?
1. What are the three steps in the deployment process?

---

# MNIST Basics


---

# 
---
toc: false
layout: post
categories: [markdown, questionnaire]
title: Q01 Introduction
---

# Introduction

1. Do you need these for deep learning?

   - Lots of math T / F: **False**, a lot of libraries have been created to take care of the complex math parts and allow us to focus on training models
   - Lots of data T / F: **False**, a lot of great results have been seen with small amounts of data
   - Lots of expensive computers T / F: **False**, there are a lot of free and cheap options available to create and deploy deep learning models
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
	- ![]({{ site.baseurl }}/images/ArthurSamuelModel.png "Arthur Samuel's Model")
1. Why is it hard to understand why a deep learning model makes a particular prediction?
    - The Deep learning models usually sift through enormous amounts of data to find data and patterns that may not be noticed by human experts. These patterns are usually difficult to isolate and make sense of in isolation and might by confusing to interpret.
1. What is the name of the theorem that shows that a neural network can solve any mathematical problem to any level of accuracy?
    - Universal approximation theorem
1. What do you need in order to train a model?
    - Data, a set of weights and 
1. How could a feedback loop impact the rollout of a predictive policing model?
    - This model will predict where more arrests will be made. If there is a bias in the data collection, the model will predict those areas where previous arrests had been high. After seeing these results, the police departments may assign more policemen to patrol areas which have a high probability of arrests which may cause even more arrests being made.
1. What is the difference between classification and regression?
    - Classification involves predicting discrete classes which the elements belong into and regression involves predicting a continuous variable for a given set of independent variables.
1. What is a validation set? What is a test set? Why do we need them?
	- While training a deep learning model, we usually train the model on a fraction of the training data and do not show the rest of the data to the model while training. The segment of data not shown to the model during training is called a validation set. It is used to measure the accuracy of the model. Another portion of the data is used to evaluate the performance of the model, this data is kept away from the model until all the hyper-parameters are tuned and modelling phases are completed. The evaluation on the final test set gives us a final assessment of our model. 	
1. What will fastai do if you don't provide a validation set?
    - Automatically create a validation set with 20% of the training data.
1. Can we always use a random sample for a validation set? Why or why not?
	- No. Sometimes if we are dealing with time series data, using random samples for a validation set will cause misleading results.
1. What is overfitting? Provide an example.
    - Training a model so that it remembers specific features of the input data, rather than generalizing well to data not seen during training
1. What is a metric? How does it differ from "loss"?
	- A metric is a measure by which we can assess hot the model is performing on the validation set. Loss is a measure of how good the model is. The metric is used for the users to understand the model while the loss is what the computer uses during the training phase to define what steps need to be taken.
1. How can pretrained models help?
    - Pretrained models can help in reducing the time taken for training and 
1. What is the "head" of a model?
	- That specific part of the model added to be specific to a particular dataset is called the head of the model
1. What kinds of features do the early layers of a CNN find? How about the later layers?
	- The early layers of the CNN identified vertical, diagonal and horizontal lines. Later layers identified repeating lines, circles and increasingly complex patterns.
1. Are image models only useful for photos?
    - No, sounds have been transformed to images based on their frequencies/loudness and then passed on to image models to identify the type of sound.
1. What is an "architecture"?
    - Architecture refers to the template of the model that we’re trying to fit; i.e., the actual mathematical function that we’re passing the input data and parameters to
1. What is segmentation?
	- Creating a model that can identify distinct objects (vehicles, pedestrians etc.) in a picture is called segmentation.
1. What is `y_range` used for? When do we need it?
    - `y_range` is a parameter that defines the range of values the prediction(target) can take.
1. What are "hyperparameters"?
	- Hyperparameters are basically parameters about parameters. They affect how fast and accurate the deep learning model performs
1. What's the best way to avoid failures when using AI in an organization?
	- Make sure the model is generalized, scalable and works on data not used to train the model. Another useful method is to use a simple model and compare the performance of the "expert" model with the simple baseline to get a sense of the accuracy of the model.

---


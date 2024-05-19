# ChatFlow

[![Static Badge](https://img.shields.io/badge/nltk-blue)](https://www.nltk.org/)
[![Static Badge](https://img.shields.io/badge/LancasterStemmer-green)](https://www.nltk.org/_modules/nltk/stem/lancaster.html)
[![Static Badge](https://img.shields.io/badge/tensorflow--saver-orange)](https://www.tensorflow.org/api_docs/python/tf/train/Saver)
[![Static Badge](https://img.shields.io/badge/numpy-red)](https://numpy.org/doc/stable/)
[![Static Badge](https://img.shields.io/badge/tflearn-purple)](http://tflearn.org/)
[![Static Badge](https://img.shields.io/badge/tensorflow-teal)](https://www.tensorflow.org/)
[![Static Badge](https://img.shields.io/badge/random-yellow)](https://docs.python.org/3/library/random.html)
[![Static Badge](https://img.shields.io/badge/json-pink)](https://docs.python.org/3/library/json.html)
[![Static Badge](https://img.shields.io/badge/pickle-brown)](https://docs.python.org/3/library/pickle.html)


The project uses natural language processing (NLP) to create a chatbot capable of understanding and responding to user queries. The chatbot is trained on a dataset of intents, which are predefined categories of user inputs. The data is preprocessed, tokenized, and transformed into numerical vectors using a bag-of-words approach. A neural network model is constructed using TensorFlow and TFLearn libraries, trained using softmax activation function and categorical cross-entropy loss.

## Table of Contents

- [About](#about)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Rating: 7/10](#Rating)

# About

The project aims to create a chatbot that can understand and respond to user queries using natural language processing (NLP) techniques. The chatbot is trained on a dataset of intents, which are predefined categories of user inputs. The training data consists of patterns and corresponding tags, representing user inputs. The project begins by preprocessing the data, tokenizing the patterns into individual words, and stemming them using the Lancaster stemming algorithm. The words are then transformed into numerical vectors using a bag-of-words approach, with labels one-hot encoded to represent different intents. A neural network model is constructed using TensorFlow and TFLearn libraries, and trained on the preprocessed data using the softmax activation function and categorical cross-entropy loss. The model is saved for future use.

# Features

The chatbot project uses natural language processing (NLP) techniques to understand user queries and provide relevant responses based on predefined intents. The chatbot is trained on a dataset of predefined intents, which represent different categories of user inputs. Data preprocessing involves tokenization, stemming, numerical representation of words, and one-hot encoding for intent labels. A neural network model is constructed using TensorFlow and TFLearn libraries, with layers for input, hidden, and output. Activation and loss functions are used. The model is trained on the preprocessed data, learning to associate patterns with specific intents. The trained model is saved for future use. Overall, this chatbot project leverages NLP techniques to understand user queries and provide relevant responses based on predefined intents.

# Installation

1) HTTPS - https://github.com/{User}/ChatFlow.git
2) CLONE - git@github.com:{User}/ChatFlow.git

# Usage

This GitHub script is designed to build and train a chatbot model using natural language processing (NLP) techniques and machine learning. It imports various libraries such as nltk, LancasterStemmer, tensorflow, tflearn, numpy, random, json, and pickle for data handling and serialization.

The script loads training data from an intents.json file, tokenizing and stemming text patterns and applying stemming to normalize words. The data is then converted into numerical arrays and output labels. The script saves the preprocessed data into a data.pickle file to avoid repeated preprocessing. If the pickle file exists, the script loads the data.

The neural network architecture is defined using tflearn, which consists of input layers, fully connected layers, and an output layer with a softmax activation function for classification. The script trains the model using the preprocessed training data and saves it to a file (model.tflearn) to avoid retraining. If the model file does not exist, it trains the model and then saves it.

The script uses various libraries to handle different tasks, including nltk for natural language processing, tflearn and tensorflow for building and training the neural network, numpy for numerical operations, random, json, and pickle for data handling and serialization.

The neural network is built using tflearn, consisting of an input layer matching the size of the training data, two hidden layers with 8 units each, and an output layer with a softmax activation function for classification. After training, the model is saved to a file to avoid retraining in future runs.

The script loads the trained model file if it exists, or trains it and saves it if it does not. This ensures that the model is trained only once and can be reused efficiently.

# Rating

The code is an implementation of a simple neural network model using TensorFlow and tflearn to train a chatbot based on intents defined in a JSON file. It has several advantages, including functionality, error handling, modularity, clarity, and reusability. However, it has some cons, such as the use of a blanket `except` clause without specifying the exact exceptions to catch, the use of magic numbers, comments, validation and testing, and the fixed neural network architecture.
To improve the code, it is suggested to refine exception handling, use named constants, add comments, implement validation, experiment with different architectures, add error handling for file operations, and document the data format expected in the JSON file and preprocessing steps performed on the data for clarity and reproducibility.
The code's performance can be improved by specifying the exact exceptions to catch in the `except` blocks, replacing magic numbers with named constants, adding comments to explain complex operations or key steps, implementing validation steps to evaluate the model's performance on a separate validation set, and experimenting with different neural network architectures, activation functions, and hyperparameters to optimize model performance for the chatbot task.
Additionally, it is suggested to add error handling for file operations and TensorFlow operations to provide more informative error messages in case of failures. Documenting the data format expected in the JSON file and the preprocessing steps performed on the data can also enhance readability and reproducibility.

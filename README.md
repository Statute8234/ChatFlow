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
- [Contributing](#contributing)
- [License](#license)

## About

The project aims to create a chatbot that can understand and respond to user queries using natural language processing (NLP) techniques. The chatbot is trained on a dataset of intents, which are predefined categories of user inputs. The training data consists of patterns and corresponding tags, representing user inputs. The project begins by preprocessing the data, tokenizing the patterns into individual words, and stemming them using the Lancaster stemming algorithm. The words are then transformed into numerical vectors using a bag-of-words approach, with labels one-hot encoded to represent different intents. A neural network model is constructed using TensorFlow and TFLearn libraries, and trained on the preprocessed data using the softmax activation function and categorical cross-entropy loss. The model is saved for future use.

## Features

• **Utilizes** natural language processing (NLP) to understand user queries.
• **Trains** chatbot on predefined intent dataset.
• **Data** preprocessing includes tokenization, stemming, numerical representation, and one-hot encoding.
• **Constructs** neural network model using TensorFlow and TFLearn libraries.
• **Uses** activation and loss functions.
• **Trains** model on preprocessed data to associate patterns with specific intents.
• **Saves** trained model for future use.

## Installation

To install ChatFlow, follow these steps:
1. Clone the repository using HTTPS:
   ```bash
   git clone https://github.com/{User}/ChatFlow.git
   ```
2. Alternatively, clone using SSH:
   ```bash
   git clone git@github.com:{User}/ChatFlow.git
   ```
3. Navigate to the project directory:
   ```bash
   cd ChatFlow
   ```

## Usage

• Utilizes natural language processing (NLP) and machine learning techniques.
• Imports libraries like nltk, LancasterStemmer, tensorflow, tflearn, numpy, random, json, and pickle for data handling and serialization.
• Loads training data from an intents.json file, tokenizing and stemming text patterns, and normalizing words.
• Converts data into numerical arrays and output labels.
• Saves preprocessed data into a data.pickle file to avoid repeated preprocessing.
• Defines neural network architecture using tflearn, consisting of input layers, fully connected layers, and an output layer.
• Trains model using preprocessed training data and saves it to a file (model.tflearn) to avoid retraining.
• Trains model and saves it if model file does not exist, ensuring efficient reuse.

## Contributing

Contributions are welcome! To contribute to Monster Maze, follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/YourFeature
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/YourFeature
   ```
5. Create a new Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

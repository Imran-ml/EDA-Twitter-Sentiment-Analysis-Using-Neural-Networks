# EDA: Twitter Sentiment Analysis Using NN

## Table of Contents

- [Introduction](#introduction)
- [Environment Setup](#environment-setup)
- [Installation Instructions](#installation-instructions)
- [Resources](#resources)
- [License](#license)
- [Conclusion](#conclusion)
- [About Author](#about-author)

## Introduction

Millions of people are using Twitter and expressing their emotions like happiness, sadness, angry, etc. The Sentiment analysis is also about detecting the emotions, opinion, assessment, attitudes, and took this into consideration as a way humans think. Sentiment analysis classifies the emotions into classes such as positive or negative. Nowadays, industries are interested to use textual data for semantic analysis to extract the view of people about their products and services. Sentiment analysis is very important for them to know the customer satisfaction level and they can improve their services accordingly. To work on the text data, they try to extract the data from social media platforms. There are a lot of social media sites like Google Plus, Facebook, and Twitter that allow expressing opinions, views, and emotions about certain topics and events. Microblogging site Twitter is expanding rapidly among all other online social media networking sites with about 200 million users. Twitter was founded in 2006 and currently, it is the most famous microblogging platform. In 2017 2 million users shared 8.3 million tweets in one hour. Twitter users use to post their thoughts, emotions, and messages on their profiles, called tweets. Words limit of a single tweet has 140 characters. Twitter sentiment analysis based on the NLP (natural language processing) field. For tweets text, we use NLP techniques like tokenizing the words, removing the stop words like I, me, my, our, your, is, was, etc. Natural language processing also plays a part to preprocess the data like cleaning the text and removing the special characters and punctuation marks. Sentimental analysis is very important because we can know the trends of people’s emotions on specific topics with their tweets.

### Problem Description/Definition

To devise a sentimental analyzer for overcoming the challenges to identify the twitter tweets text sentiments (positive, negative) by implementing neural network using tensorflow.

### Evolution Measures

After training the model, we apply the evaluation measures to check that how the model is getting predictions. We will use the following evaluation measures to evaluate the performance of the models:
    <li>Accuracy</li>
    <li>Confusion matrix with plot</li>
    <li>ROC Curve</li>

### Technical Approach

We are using python language in the implementations and Jupter Notebook that support the machine learning and data science projects. We will build tensorflow based model. We will use Sentiment 140 dataset and split that data into 70% for training and 30% for the testing purposes. After training on the model, we will evaluate the model to evaluate the performance of trained model.

### Implementing Tensorflow Based Model for Training

<h4> Step 1</h4>
- The input to model is 500 words because these are the number features/words that we extracted above from text of tweets.

<h4> Step 2</h4>
- Embeddings provide the presentation of words and their relative meanings. Like in this, we are feeding the limit of maximum words, lenght of input words and the inputs of previous layer. 

<h4> Step 3</h4>
- LSTM (long short term memory) save the words and predict the next words based on the previous words. LSTM is a sequance predictor of next coming words.

<img src="https://static.wixstatic.com/media/3eee0b_969c1d3e8d7943f0bd693d6151199f69~mv2.gif">
<h4> Ref: https://static.wixstatic.com/media/3eee0b_969c1d3e8d7943f0bd693d6151199f69~mv2.gif </h4>

<h4> Step 4</h4>
- Dense layer reduce the outputs by getting inputs from Faltten layer. Dense layer use all the inputs of previous layer neurons and perform calculations and send 256 outputs

<h4> Step 5</h4>
- Activation function is node that is put at the end of all layers of neural network model or in between neural network layers. Activation function help to decide which neuron should be pass and which neuron should fire. So activation function of node defines the output of that node given an input or set of inputs. 

<img src="https://miro.medium.com/v2/resize:fit:1400/1*mcJfRvd9zarAbkHppFRrCQ.gif">
<h4> Ref: https://miro.medium.com/v2/resize:fit:1400/1*mcJfRvd9zarAbkHppFRrCQ.gif </h4>

<h4> Step 6</h4>
- Droupout layer drop some neurons from previous layers. why we apply this? We apply this to avoid the overfitting problems. In overfitting, model give good accuracy on training time but not good on testing time.
<img src="https://i.imgur.com/a86utxY.gif">
<h4> Ref: https://i.imgur.com/a86utxY.gif </h4>

## Environment Setup

**Prerequisites**: Ensure Python 3.6 or newer is installed on your system.

1. **Create a Virtual Environment**:
    - Install `virtualenv` if you prefer it over the built-in `venv` (optional):
        ```bash
        pip install virtualenv
        ```
    - Create the environment:
        - With `venv` (Python 3.3+):
            ```bash
            python -m venv env
            ```
        - Or, with `virtualenv`:
            ```bash
            virtualenv env
            ```
    - Activate the environment:
        - Windows: `env\Scripts\activate`
        - Unix/MacOS: `source env/bin/activate`
    - To deactivate: `deactivate`

2. **Dependencies**:
    Ensure all dependencies are listed in `requirements.txt`. Install them using:
    ```bash
    pip install -r requirements.txt
    ```

## Installation Instructions

To use this project, clone the repository and set up the environment as follows:

1. **Clone the Repository**:
    ```bash
    https://github.com/Imran-ml/EDA-Twitter-Sentiment-Analysis-Using-NN.git
    ```
2. **Setup the Environment**:
    - Navigate to the project directory and activate the virtual environment.
    - Install the dependencies from `requirements.txt`.

## Resources

- **Kaggle Notebook**: [View Notebook](https://www.kaggle.com/code/muhammadimran112233/eda-twitter-sentiment-analysis-using-nn)
- **Dataset**: [View Dataset](https://www.kaggle.com/datasets/kazanova/sentiment140)

## License

This project is made available under the MIT License.

## Conclusion

We used the twitter sentiment analysis dataset and explored the data with different ways:
        <li>We prepared the text data of tweets by removing the unnecessary things.</li>
        <li>We trained model based on tensorflow with all settings. </li>
        <li>We evaluated thye model with different evaluation measures.</li>
        <li>If you are interested to work on any text based project, you can simply apply the same methodolgy but might be you will need to change little settings like name                 of coloumns etc.</li>
        <li>We worked on the classification problem and sepcifically we call it binary classification which is two class classification.</li>

## About Author

- **Name**: Muhammad Imran Zaman
- **Email**: [imranzaman.ml@gmail.com](mailto:imranzaman.ml@gmail.com)
- **Professional Links**:
    - Kaggle: [Profile](https://www.kaggle.com/muhammadimran112233)
    - LinkedIn: [Profile](linkedin.com/in/muhammad-imran-zaman)
    - Google Scholar: [Profile](https://scholar.google.com/citations?user=ulVFpy8AAAAJ&hl=en)
    - YouTube: [Channel](https://www.youtube.com/@consolioo)
- **Project Repository**: [GitHub Repo](https://github.com/Imran-ml/EDA-Twitter-Sentiment-Analysis-Using-NN.git)

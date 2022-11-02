# Word Embeddings and Neural Text Classifiers
For this notebook, it divived into three sections which are word embeddings, introducing neural text classifiers, improving neural text classifiers

---
## Part 1: Word Embeddings
### Overview
This provided an introduction to loading and training word embeddings using the Gensim library working with [the tweet eval sentiment](https://huggingface.co/datasets/tweet_eval) dataset [1]. 

This aimed to obtain a document embedding that characterises the meaning of a document, followed by using the embeddings to organise the tweets into topic categories. Next, it used PCA and K-Mean to visualise the words that are most strongly associated with each category. Based on those steps, it can identify five similar words for each topic.

### Objective

To identify the five similar words from word embeddings using Gensim library working with the tweet eval sentiment dataset.

---
## Part 2: Introducing Neural Text Classifiers
### Overview
This section implemented a neural network classifier using Pytorch for sentiment analysis. In this study, it took a sequence of tokens as input and predicted a class label. 

This model can handle much more complex relationships between features and class labels.  Moreover,it performed representation learning: the hidden layers learn how to extract features from low-level data.

### Objective
Adopt Pytorch to construct a neural network classifier for sentiment analysis
 
---

## Part 3: Improving Neural Text Classifiers
### Overview
Due to considering the limitations of the neural text classifier in part 2, this part improved the model as follows:

* Change the parameter; freeze=False. It can update the parameter's weight through backpropagation so the accuracy and f1 score will improve.

* Use the LSTM model. This model can process important long-distance information and have a long-term memory.

### Objective
Improve the accucary of the neural text classifier in part 2 by using 
the LSTM model and change the parameter.

---

## Reference

[1] TweetEval: Unified Benchmark and Comparative Evaluation for Tweet Classification (Barbieri et al., Findings 2020)
# Transformers

This notebook combined two parts: introducing transformers and classification with transformers 

---
## Part 1: Introducing Transformers
### Overview
This section introduces the Transformers library from HuggingFace with simple tasks to retrieve contextualised embeddings from pretrained transformer models.

### Objective
It intended to obtain contextualised word embeddings using pretrained transformers with simple problems.

---

## Part 2: Classification with transformers
### Overview
For this task, it constructed a neural network classifier using Transformers to classify the emotion analysis from [the Tweet Eval dataset](https://huggingface.co/datasets/tweet_eval) [1] into one of 0: anger, 1: joy, 2: optimism, or 3: sadness.

For this task, it constructed a neural network classifier using Transformers to classify the emotion analysis from [the Tweet Eval dataset](https://huggingface.co/datasets/tweet_eval) [1] into one of 0: anger, 1: joy, 2: optimism, or 3: sadness.  The pretrained BERT model was performed to achieve this task.

### Objective
Used BRERT model from Transformers to classify the emotion analysis dataset

---

## Reference
[1] C. Van Hee, E. Lefever, and V. Hoste, “SemEval-2018 task 3 : irony detection in English tweets,” in Proceedings of The 12th International Workshop on Semantic Evaluation, New Orleans, Louisiana, 2018, pp. 39–50.

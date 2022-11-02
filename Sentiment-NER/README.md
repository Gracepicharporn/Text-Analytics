# Sentiment Classification and Named Entity Recognition
This notebook contains sentiment classification and named entity recognition project.

---   
  
## Part1 : Sentiment Classification
### Overview
In this section, it was designed to implement and evaluate a sentiment classifier with working with [the Financial Phrasebank dataset](https://huggingface.co/datasets/financial_phrasebank) [1] which contained English news articles from financial articles on the Helsinki stock exchange. Each sentence is labelled with different three labels which are neutral (0), negative (1) or positive (2). 

For this task, it applied the text normalization methods, namely tokenization, lemmatization and lemmatization & bi-grams that transform the raw text to an input format. After those pre-processes, it converted the training and validation dataset to the bag of words by the CountVectorizer class which convert text into the feature vectors and count the words occurred in text. This was followed by using the Naïve Bayes Classifier and the Logistic Regression to classify sentences into three classes.

### Objective
This task aimed to find the appropriate feature method and the model that gave the highest f1 score.

---   

## Part2: Named Entity Recognition
### Overview
This work deloped named entity using [the SEC-Filings dataset](https://www.sec.gov/dera/data/financial-statement-data-sets.html) [2] in the U.S. financial documents to extract information automatically in this dataset about organization (ORG), person (PER), location (LOC) and miscellaneous (MISC).

Named Entity Recognition (NER) identified the tag of each word including organization, location, and person. In the NER, it showed the entity type of each span, which was a sub-sequence by tokenization from the text, and the boundary of each span including B- (beginning of span), I- (Inside an entity span) and O (not an entity). For example, I-ORG meant that this word is inside an entity span and the organization type. There are three approaches to pre-process this dataset that is unigram and unigram & adding some features and part of speech tagging (POS). Next, it used the Condition random field (CRF) to predict the named entity recognition tag for each word. 

### Objective
This study focused on exploring multiple feature extraction methods using CRF to obtain the best accuracy for this task.

--- 

## Part 3: Perform the trained NEG tagger to the Financial Phrasebank dataset

In this task, it applied the CRF model and NEG tagger with Part of Speech Tagging (POS) feature from the previous section to the Financial Phrasebank dataset from part1 because this feature gave the higher performance of F1 score. 

The purpose was to compute a sentiment score for each entity that was detected from this dataset and returned the five most positive and five most negative sentences.

---

## Reference 

[1] Malo, Pekka et al. “Good debt or bad debt: Detecting semantic orientations in economic texts.” Journal of the Association for Information Science and Technology 65 (2014)

[2] Data. SEC Emblem. (2009, January 1). Retrieved October 31, 2022, from https://www.sec.gov/dera/data/financial-statement-data-sets.html 
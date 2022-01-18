---
title: NLP-Project-Phone-Review-Analysis-and-Topic-Modelling-with-Latent-Dirichlet-Allocation-in-Python
date: 2021-12-20 3:21:00 +0530 
tags: [Machine learning, Python, Natural Language Processing, Topic Modelling, Latent Dirchlet Allocation, POS-Tagging, numpy, pandas, nltk, gensim, matplotlib, pyLDAvis]
comments: false
img_path: /assets/img/2021-12-20-NLP-Project-Phone-Review-Analysis-and-Topic-Modelling-with-Latent-Dirichlet-Allocation
---

### Summary-

This is a Natural Language Processing project which includes analysis of buyer's reviews/comments of a popular mobile phone by Lenovo from an e-commerce website. Analysis done for the project include pre-processing of text data such as word-tokenisation, lemmatisation.  
This is followed by Topic-modelling using Latent Dirichlet Allocation, POS tagging, and topic interpretation for business use

You can view the full project code on this [Github link](https://github.com/Ransomk/NLP-Course-Project-Review-Analysis-and-Topic-Modelling-with-LDA)

Note: _This is an academic project completed by me as part of my Post Graduate program in Data Science from Purdue University through Simplilearn. This project was towards the completion of Data Science Natural Language Processing (NLP)module._

### Bussiness Scenario

### Objective

### Analysis Steps
1. Read the .csv file using Pandas. Take a look at the top few records.
2. Normalize casings for the review text and extract the text into a list for easier manipulation.
3. Tokenize the reviews using NLTKs word_tokenize function.
4. Perform parts-of-speech tagging on each sentence using the NLTK POS tagger.
5. For the topic model, we should want to include only nouns.
    A. Find out all the POS tags that correspond to nouns.
    B. Limit the data to only terms with these tags.
6. Lemmatize.
    A. Different forms of the terms need to be treated as one.
    B. No need to provide POS tag to lemmatizer for now.
7. Remove stopwords and punctuation (if there are any).
8. Create a topic model using LDA on the cleaned-up data with 12 topics.
    A. Print out the top terms for each topic.
    B. What is the coherence of the model with the c_v metric?
9. Analyze the topics through the business lens.
    A. Determine which of the topics can be combined.
10. Create topic model using LDA with what you think is the optimal number of topics
    A. What is the coherence of the model?
11. The business should be able to interpret the topics.
    A. Name each of the identified topics.
    B. Create a table with the topic name and the top 10 terms in each to present to the business.


### Tools used:
This project was completed in Python using Jupyter notebooks.
Common libraries used for analysis include numpy, pandas, nltk, gensim, matplotlib, pyLDAvis

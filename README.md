# Self-supervised_Topic_classification
A major task in NLP application is to identify topics. It gets more complex to deal with topics as the texts get short. This project aims to tackle the topic classification problem using self supervised learning.

Dataset used : 
  1. Garage review dataset: Contains reviews of users who availed a garage service.
  2. Evaluation labels: Contains number of topics that the reviews can be classified into.

There are two ipynb files:
  1. Topic_modelling.ipynb : Unsupervised way of finding topics in a corpus of text.
  2. Topic_classification.ipynb : Supervised learning for topic classification.

For unsupervised topic modeling, LDA (Latent Dirichlet allocation) is used which is a popular Topic modeling technique. 
https://en.wikipedia.org/wiki/Latent_Dirichlet_allocation
The output of LDA model is a list of cluster of words where each cluster denotes a particular topic. The more the words are related in each cluster, better is the result.

LDA 2-Dimensional topic visualization using pyLDAvis:
![Untitled](https://user-images.githubusercontent.com/36213156/133375211-3c2ef05d-a595-450b-a4cf-52a5eecd8466.png)

Finally after labelling each cluster into pre-defined topics from the list of topics, we use classification models to verify the final result. Can be found in Topic_classification.ipynb. 

![Untitled](https://user-images.githubusercontent.com/36213156/133376470-4586a060-84a6-44f0-9b6b-e105ccd853a2.png)




# Named Entity Recognition

## 1. Introduction

In this project, we are interested in the study of Named Entity Recognition (NER) which is a subtask of information extraction that seeks to locate and classify named entity mentioned in unstructured text into pre-defined categories such as person names, organizations, locations... In this project, we are interessted in comparing the performence of classical machine learning approaches, e.g. Conditional Random Fields (CRF), and neural network based methods on the task of NER tagging. 

## 2.Datasets :
We use two different datasets to compare the different approaches for NER tagger

  * CoNLL-2002 [1]: 
  * CoNLL-2003 [2]:
  * NER in Tweets [3]:
  
## 3.Exerimental Sertings:
### Nerual NER tagger:
We use a simple model to build the NER tagger, the proposed model  has only tree layers, an embedding layer that transforms the indexe into vectors, the second layer is an LSTM layer and the last layer is a Linear layer that maps the output of the LSTM layer to the required dimension, i.e. the number of all possible tags. All those layers are implemented in pytorch and can be used easily. We used Adam optimizer with learning rate 0.005, and we used a batch size of 32, we used an embedding space of size 128. All the training was done on GPU, Nividia Geforce GTX 1050.

## 4.Results :


## 5.Requirements :
* PyTorch
* Numpy
* Tensorboard

## 6. References
[1] *Introduction to the CoNLL-2002 Shared Task: Language-Independent Named Entity Recognition,* Erik F. and Tjong Kim Sang. 

[2] *Introduction to the CoNLL-2003 Shared Task: Language-Independent Named  Recognition,* Erik F. Tjong Kim Sang and Fien De Meulder.

[3] *Named Entity Recognition in Tweets: An Experimental Study* Alan Ritter, Sam Clark, Mausam and Oren Etzioni.
    

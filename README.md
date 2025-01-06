# Ma513-NER for Cyber Security Project

This repository contains the implementation of two Named Entity Recognition (NER) systems for the domain of Cybersecurity, developed as part of the Statistical Learning course at IPSA. In this project we designed and trained two NER models, one using Logistic Regression and one using a pretrained model (BERT), capable of identifying domain-specific entities such as actions, modifiers and entities.

We used the IOB2 syntax for the tags and the dataset used is titled "Semantic Extraction from Cybersecurity Reports using Natural Language Processing (SecureNLP)" which contains technical cybersecurity documents. The dataset is already separated for training (NER-TRAINING.jsonl), validation (NER-VALIDATION.jsonl) and testing (NER-TESTING.jsonl). 

To obtain results we preprocessed the data, trained the models and did predictions of the ner-tags on the testing file but also on the validation file. The predictions on the validation file allowed us to compare them with ner-tags already present in the validation file and this way we calculated different scores like the precision, the recall and the F1 score to estimate the accuracy of our models.

Each Jupyter Notebook corresponds to a model and once every cell have been run in each of them, a save of the model as well as two prediction files (one for validation set and the other for the testing set) will be produced and saved in the current directory:
- The model checkpoint will be usefull if we don't want to go through the trainning of the model again, we can just charge the save
- The two prediction files are the files used to calculate the scores at the end of each Notebook, make sure to change the file name as indicated in the code

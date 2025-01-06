# Ma513-NER for Cyber Security Project

This repository contains the implementation of two Named Entity Recognition (NER) systems for the domain of Cybersecurity, developed as part of the Statistical Learning course at IPSA. In this project we designed and trained two NER models, one using Logistic Regression and one using a pretrained model (BERT), capable of identifying domain-specific entities such as actions, modifiers and entities.

We used the IOB2 standard and the dataset used is "SemEval-2018 Task 8", titled "Semantic Extraction from Cybersecurity Reports using Natural Language Processing (SecureNLP)" which contains technical cybersecurity documents. The dataset is already separated for training (NER-TRAINING.jsonl), validation (NER-VALIDATION.jsonl) and testing (NER-TESTING.jsonl). 

To obtain results we preprocessed the data, trained the models and did predictions of the ner-tags on the testing file but also on the validation file. The predictions on the validation file allowed us to compare them with ner-tags already present in the validation file and this way we calculated different scores like the precision, the recall and the F1 score to estimate the accuracy of our models.

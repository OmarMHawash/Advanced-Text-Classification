# Advanced Text Classification Project

## Overview

This project aims to classify news documents into 91 different classes using various text classification models and techniques. The report covers the methodology, performance comparison, and suggestions for enhancements.

if you want full repoert, here : [Results Report](docs/report.pdf)

## Author

- **Omar Hawash**
- Date: 14.04.2024
- NLP Course - AN-Najah National University
- Supervisor: Dr. Hamed Abdelhaq

## Introduction

Text classification is a fundamental task in natural language processing (NLP) that involves categorizing text documents into predefined classes or categories. In this project, we explore advanced text classification techniques to achieve high accuracy and F1-Score.

### Hypothesis

- **Dataset**: News documents with body text and 91 different classes.
- **Training Data**: 11413 samples
- **Testing Data**: 4024 samples

## Materials

1. Naive Bayes theoretical equation
2. Sk-learn pre-trained models
3. Gensim pre-trained models

## Procedure

### Models Accuracy

#### A. Naive Bayes

| Model          | Mean Average F1-Score (%) |
| -------------- | ------------------------- |
| Naive Bayes_01 | 3.57                      |
| Naive Bayes_02 | 3.63                      |
| Naive Bayes_03 | 3.48                      |

#### B. Scikit-learn Naive Bayes

| Model                  | Mean Average F1-Score (%) |
| ---------------------- | ------------------------- |
| Sk_learn Count Vector  | 30.73                     |
| Sk_learn TF-IDF Vector | 13.73                     |

#### C. Word Embedding Models

| Model    | Mean Average F1-Score (%) |
| -------- | ------------------------- |
| Glove    | 26.67                     |
| Word2Vec | 15.96                     |
| FastText | 5.03                      |
| Glove_02 | 35.7                      |
| Glove_03 | 37.73                     |

#### D. SVM & Random Forest

| Model         | Mean Average F1-Score (%) |
| ------------- | ------------------------- |
| SVM           | 36.78                     |
| Random Forest | 22.66                     |

## Results

- Naive Bayes models achieved accuracies around 50% and F1-Scores near 3.5%.
- Scikit-learn Naive Bayes CountVectorizer model outperformed TF-IDF in F1-Score.
- Word Embedding Models, particularly Glove, achieved the highest performance with a mean average F1-Score of 37.73%.
- Changing the solver of logistic regression had a negligible effect on results.

## Conclusion

Despite various preprocessing and model selection techniques, the performance of the models varied. Word embedding models, especially Glove, showed promising results. Further enhancements could include exploring different preprocessing methods and experimenting with deep learning architectures.s

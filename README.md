# toxic_comment_classifier
Problem Statement and Background

Discussing things you care about can be difficult. The threat of abuse and harassment online means that many people stop expressing themselves and give up on seeking different opinions. Platforms struggle to effectively facilitate conversations, leading many communities to limit or completely shut down user comments.

The exact problem statement was thus as below:

Given a group of sentences or paragraphs, used as a comment by a user in an online platform, classify it to belong to one or more of the following categories — toxic, severe-toxic, obscene, threat, insult or identity-hate with either approximate probabilities or discrete values (0/1).

Data and Model used:

The Dataset used for this task is sourced from a Kaggle competition and is titled as the Jigsaw/Conversation AI Toxic Comment Classification Challenge Dataset. The creator have so far built a range of publicly available models served through the Perspective API and created this competition to enable participants to build a multi-headed model that is capable of detecting different types of toxicity like threats, obscenity, insults, and identity based hate better than their models. The dataset is composed of comments from Wikipedia’s talk page edits. The various categorizations for the comments are: toxic, severe toxic, obscene, threat, insult, and identity hate.The training dataset consists of 160k training samples and the test set consists of 153k samples.Understanding the dataset is an extremely vital task and there are several insights to be drawn from the dataset.

There were various models which could have been used but in my approach i used logistic Regression along with Tf-Idf. Tf-Idf stands for term frequency-inverse document frequency, and instead of calculating the counts of each word in each document of the dataset , it calculates the normalized count where each word count is divided by the number of documents this word appears. I’ve applied logistic regression which is a classification algorithm used to solve binary classification problems. The logistic regression classifier uses the weighted combination of the input features and passes them through a sigmoid function. Sigmoid function transforms any real number input, to a number between 0 and 1.

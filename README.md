# Spam_Detection
In this project we'll build a model that classifies messages as spam or non-spam using Naive Bayes Algorithm.

Naive Bayes theorem is a probabilistic model used in text classification to calculate the probability of a given document belonging to a particular label, based on the occurrence of its features or words. In email spam classification, we have two labels, "Ham" and "Spam". 
The algorithm learns the probabilities of each feature or word occurring in each label, and for a new text, calculates the likelihood of each label based on the occurrence of its features or words. It selects the label with the highest posterior probability as the final result. Naive Bayes is an efficient and effective method for text classification, especially in cases where the dataset is sparse and the number of features or words is large.

## Calculating Probabilities

$$P(spam|word_1, word_2,\dots , word_n) \propto P(spam)\cdot \prod_{i = 1}^{n}P(word_i|spam)$$
$$P(non\ spam|word_1,word_2,\dots , word_n) \propto P(non\ spam)\cdot \prod_{i = 1}^{n}P(word_i|non\ spam)$$
$$P(word_i|spam) = \frac{X_i + \alpha}{N + \alpha \cdot d}$$ where $X_i$ is represents the frequency of $word_i$ in a spam message, $\alpha$ is the smoothing parameter (we'll set it to 1), $N$ is the number of words in the spam set, $d$ is the number of words in our vocabulary. The same is applied when we condition on "non-spam" messages.

##Brief
We have seamlessly merged the frontend and Python backend components by harnessing the power of Flask, a cutting-edge micro web framework.
##Preview
---
http://bablu123.pythonanywhere.com/
---

# Multi-label classification project

---

### Introduction :
In a multi-label classification problem, each sample can belong to multiple classes or labels. This is different from a traditional single-label classification problem, where each sample can only belong to one class or label. Common approaches to solving multi-label classification problems include binary relevance, classifier chains, and label powerset. These methods can be used in conjunction with traditional machine learning algorithms, such as decision trees, random forests, and neural networks.

---

### EDA :
EDA is typically the first step in the data analysis process and is used to gain insight into the data and to identify potential issues or outliers.

---

### Binary Relevance Classifier :
Binary Relevance (BR) is a simple and widely used method for solving multi-label classification problems. The basic idea behind the BR method is to train a separate binary classifier for each label, where each classifier is trained to predict the presence or absence of a specific label in a given sample.
The BR method is simple to implement and can be used with any binary classifier, such as logistic regression, decision trees, and support vector machines (SVMs). The BR method can also be easily combined with other feature selection or feature transformation methods. One of the main limitations of the BR method is that it does not take into account the relationships between labels, which can lead to suboptimal performance in some cases.

---

### Binary Relevance Classifier with Under-Sampling:
Binary Relevance (BR) with Under-Sampling is a method for solving multi-label classification problems that combines the BR method with under-sampling techniques. Under-sampling is a technique used to balance the class distribution in a dataset by removing samples from the majority class.
The basic idea behind BR with Under-sampling is to first under-sample the majority class in each binary classification problem, and then train a separate binary classifier for each label using the under-sampled dataset. By under-sampling the majority class, the classifiers are able to better focus on the minority class, which can improve the overall performance of the BR method. One of the main limitations is that it can lead to a loss of information by removing samples from the majority class, which can negatively impact the overall performance of the method.


---

### Classifier Chains:
Classifier Chains (CC) is a method for solving multi-label classification problems that uses a chain of binary classifiers. The basic idea behind the CC method is to train a sequence of binary classifiers, where each classifier is trained to predict the presence or absence of a specific label, and the output of each classifier is used as input to the next classifier in the chain.
The first classifier in the chain is trained to predict the presence or absence of the first label, and its output is used as input to the second classifier, which is trained to predict the presence or absence of the second label, and so on. This creates a chain of classifiers where each classifier is conditioned on the outputs of the previous classifiers. One of the main limitations of the CC method is that it can be sensitive to the order of the labels in the chain, which can lead to suboptimal performance if the wrong order is chosen.

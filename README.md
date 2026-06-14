#  Edible vs Poisonous Mushroom Classification using a Decision Tree (From Scratch)

## Overview

This project implements a **Decision Tree Classifier from scratch using Python and NumPy** to classify mushrooms as **edible** or **poisonous**.

Instead of relying on machine learning libraries such as Scikit-Learn, the goal was to understand the underlying mathematics and algorithms that power decision trees, including entropy calculation, information gain, feature selection, and recursive tree construction.

This project was completed as part of my machine learning learning journey to strengthen my understanding of supervised learning algorithms.

---

## Problem Statement

Given a set of mushroom characteristics represented as binary features, determine whether a mushroom is:

* **Edible (1)**
* **Poisonous (0)**

The classifier learns decision rules by selecting the feature that maximizes information gain at each split.

---

## Dataset

The dataset consists of 10 mushroom samples with 3 binary features:

| Feature Index | Description          |
| ------------- | -------------------- |
| 0             | Brown Cap            |
| 1             | Tapering Stalk Shape |
| 2             | Solitary             |

Target labels:

| Label | Meaning   |
| ----- | --------- |
| 1     | Edible    |
| 0     | Poisonous |

---

## Machine Learning Concepts Implemented

### 1. Entropy

Entropy measures the uncertainty or impurity of a dataset.

A node containing a mix of edible and poisonous mushrooms has higher entropy than a node containing only one class.

### 2. Information Gain

Information Gain quantifies how much uncertainty is reduced after splitting the dataset on a particular feature.

The feature with the highest information gain is selected for splitting.

### 3. Feature Selection

Each feature is evaluated and compared based on its information gain.

The algorithm automatically chooses the most informative feature.

### 4. Recursive Tree Building

The tree is built recursively until a predefined maximum depth is reached.

---

## Project Workflow

1. Load training data
2. Compute entropy of the current node
3. Evaluate all possible feature splits
4. Compute information gain for each split
5. Select the best feature
6. Split the dataset into child nodes
7. Recursively repeat the process
8. Stop when maximum depth is reached

---

## Project Structure

```text
├── EdibleorPoisonous.ipynb
├── public_tests.py
└── README.md
```

---

## Skills Demonstrated

* Machine Learning Fundamentals
* Decision Tree Algorithms
* Information Theory
* Recursive Programming
* Algorithm Design
* Data Manipulation with NumPy
* Problem Solving
* Model Interpretation

---

## Technologies Used

* Python
* NumPy
* Matplotlib
* Google Colab

---

## Sample Output

```text
Depth 0, Root: Split on feature: 2
- Depth 1, Left: Split on feature: 0
-- Left leaf node with indices [0, 1, 4, 7]
-- Right leaf node with indices [5]
- Depth 1, Right: Split on feature: 0
-- Left leaf node with indices [2, 3, 9]
-- Right leaf node with indices [6, 8]
```

---

## Key Takeaways

Through this project, I gained practical experience with:

* How decision trees determine optimal splits
* The role of entropy in measuring uncertainty
* Information gain as a feature selection criterion
* Recursive tree construction
* Building machine learning algorithms without external ML frameworks

---

## Future Improvements

* Add prediction functionality for unseen samples
* Visualize the generated decision tree
* Support continuous numerical features
* Implement pruning techniques
* Compare performance with Scikit-Learn's DecisionTreeClassifier
* Extend to larger real-world datasets

---

## About Me

I am a Computer Science undergraduate interested in Machine Learning, Data Science, and Artificial Intelligence. I enjoy implementing algorithms from scratch to build a deeper understanding of how machine learning models work internally.

Feel free to connect with me or explore my other projects.

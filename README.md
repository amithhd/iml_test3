# 

## Decision Tree ID3 Algorithm

This code implements the ID3 (Iterative Dichotomiser 3) algorithm for building a decision tree. The ID3 algorithm uses the concept of information gain to construct the decision tree.

### Algorithm Steps

1. *Node Class*: The code defines a `Node` class representing the nodes in the decision tree. Each node has an attribute and a dictionary of children nodes.
2. *ID3 Algorithm*: The main function `id3` implements the ID3 algorithm. It takes the input data, target attribute, and a list of attributes as parameters. The algorithm recursively builds the decision tree by calculating information gain and selecting the best attribute at each step.
3. *Information Gain Calculation*: The function `calculate_information_gain` computes the information gain for each attribute. It calculates the entropy of the target attribute and the weighted average entropy of the attribute being considered.
4. *Entropy Calculation*: The function `calculate_entropy` calculates the entropy of a target attribute based on the frequency distribution of its classes.
5. *Sample Classification*: The function `classify_sample` classifies a new sample using the decision tree. It traverses the decision tree based on the attribute values of the sample until a leaf node is reached and returns the class label of the leaf node.
6. *Dataset Preparation*: The code prepares the dataset by creating a DataFrame using the "PlayTennis" dataset.
7. *Building the Decision Tree*: The decision tree is built by calling the `id3` function with the dataset, target attribute ("PlayTennis"), and the list of attributes.
8. *Classifying a New Sample*: A new sample is classified using the decision tree by calling the `classify_sample` function with the new sample and the decision tree. The result is printed as the classification label.

### Usage

To use this code, follow these steps:

1. Define your dataset as a pandas DataFrame, where each column represents a feature and the last column represents the target attribute.
2. Set the target attribute name and list the attribute names.
3. Call the `id3` function with the dataset, target attribute, and attribute list to build the decision tree.
4. Classify new samples by calling the `classify_sample` function with a new sample and the decision tree.

### Example

An example of using this code with the "PlayTennis" dataset:

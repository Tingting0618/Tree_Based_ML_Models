# Tree Based ML Models

## Decision Trees
Decision Trees are versatile Machine Learning algorithms that can perform both classification and regression tasks, and even multioutput tasks.

Iris example: 

![2021-07-17 21_29_11-Webgraphviz](https://user-images.githubusercontent.com/44503223/126053785-dc0098ee-7767-43fc-8c83-929c7807f668.png)

#### Decision Trees Notebook Content Includes:
- Estimating Class Probabilities
- Prevent Overfitting
  - max_depth: regularize the model and thus reduce the risk of overfitting
  - min_samples_split (the minimum number of samples a node must have before it can be split)
  - min_samples_leaf (the minimum number of samples a leaf node must have)
  - min_weight_fraction_leaf (same as min_samples_leaf but expressed as a fraction of the total number of weighted instances)
  - max_leaf_nodes (the maximum number of leaf nodes)
  - max_features (the maximum number of features that are evaluated for splitting at each node)

This repo is my learning notebook following the book:
Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow, 2nd Edition, by Aurélien Géron (O’Reilly).
Copyright 2019 Kiwisoft S.A.S., 978-1-492-03264-9.

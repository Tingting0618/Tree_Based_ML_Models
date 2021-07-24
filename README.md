# Tree Based ML Models

## 1. Decision Trees
Decision Trees are versatile Machine Learning algorithms that can perform both classification and regression tasks, and even multioutput tasks.

Iris example: 

![2021-07-17 21_29_11-Webgraphviz](https://user-images.githubusercontent.com/44503223/126053785-dc0098ee-7767-43fc-8c83-929c7807f668.png)

Here we have the 1 root node, 1 internal node, and 3 leaves. 

#### How to determine which feature should be used on the root node?
We make a decision based on the minimum Gini Impurity (i.e., largest separability).

To calculate Gini Impurity, there are 2 steps:

**Step 1**: calculate Gini score for each leaf
<img width="638" alt="Screen Shot 2021-07-24 at 8 14 09 AM" src="https://user-images.githubusercontent.com/44503223/126869547-85d58b92-a273-4350-a9b7-3e8afc8dd331.png">

**Step 2**: calculate Gini score for each node, based on a weighted average
<img width="640" alt="Screen Shot 2021-07-24 at 8 12 48 AM" src="https://user-images.githubusercontent.com/44503223/126869576-224a3678-add8-42f1-b312-c7f62d5f04d5.png">

A Decision Tree can also estimate the **probability** that an instance belongs to a particular class k. 

To **avoid overfitting**, we could:
- max_depth: regularize the model and thus reduce the risk of overfitting
- min_samples_split (the minimum number of samples a node must have before it can be split)
- min_samples_leaf (the minimum number of samples a leaf node must have)
- min_weight_fraction_leaf (same as min_samples_leaf but expressed as a fraction of the total number of weighted instances)
- max_leaf_nodes (the maximum number of leaf nodes)
- max_features (the maximum number of features that are evaluated for splitting at each node)

![download](https://user-images.githubusercontent.com/44503223/126869101-2502362d-8934-4eee-b9ac-93a29b66b27e.png)

**Limitation - Instability**
- Decision Trees are very sensitive to small variations in the training data.
- Decision Trees love orthogonal decision boundaries (all splits are perpendicular to an axis), which makes them sensitive to training set rotation.

**Solution** to Decision Trees' Limitation? - Random Forests

## Learn More

Please visit [Tingting Duan's Project Portfolio](https://tingting0618.github.io).

## Reference

This repo is my learning journal following:
- Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow, 2nd Edition, by Aurélien Géron (O’Reilly). Copyright 2019 Kiwisoft S.A.S., 978-1-492-03264-9.
- StatQuest: Decision Trees https://statquest.org/statquest-decision-trees/

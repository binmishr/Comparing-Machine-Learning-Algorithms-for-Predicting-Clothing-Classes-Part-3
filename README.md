# Comparing-Machine-Learning-Algorithms-for-Predicting-Clothing-Classes-Part-3

The details of the codeset and plots are included in the attached Microsoft Word Document (.docx) file in this repository. 
You need to view the file in "Read Mode" to see the contents properly after downloading the same

A Brief Introduction
=====================

In a series devoted to comparing different machine learning methods for predicting clothing categories from images using the Fashion MNIST data by Zalando. In the first post of this series, the data has been prepared for analysis and used my “go-to” Python deep learning neural network model to predict the clothing categories of the Fashion MNIST data. The principal components analysis (PCA) is used to compress the clothing image data down from 784 to just 17 pixels. In this post, we pick up where we left off in Part 2 and use the two data sets train.data.pca and test.data.pca to build and compare random forest and gradient-boosted models. The R code for this post can be found on my Github repository.
Tree-Based Methods

Tree-based methods stratify or segment the predictor space into a number of simple regions using a set of decision rules that can be summarized in a decision tree. The focus here will be on classification trees, as the Fashion MNIST outcome variable is categorical with ten classes. Because single trees have a relatively low level of predictive accuracy compared to other classification approaches, I will not show you how to fit a single tree in this blog post, but you can find the code for this (as well as tree pruning) on my Github.

Ensemble methods improve predictive accuracy and decrease variance by aggregating many single decision trees. Here, I show both random forests and gradient-boosted trees as ensemble methods because the former are easier to implement as they are more robust to overfitting and require less tuning, while the latter generally outperform other tree-based methods in terms of prediction accuracy. The models are estimated in supervised mode here as labeled data are available and the goal is to predict classes. For a more formal explanation of the tree-based methods, I refer you to James et al. (2013).

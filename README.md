# Computer-Vision
Project with my Computer Vision investigations 

---
## Assignment 1
This assignment is a programmic one (mostly). Your task is to implement 2D geometric transformations

1. Create a blanc canvas and put a rectangular image on the canvas (image being smaller then the canvas). Choose any image you want. NB! Include this image in the submitted work.

2. Implement the 2D transformation from the lecture (translation, Euclidean, similarity, affine, homography) (+1 points per transformation)

3. Implement inverse transformations, and explain (!) (+1 point in total)

4. Prove that geometric transformations 

a - form groups (+2 points)

b - these groups are nested (+1 point)

---

## Assignment 2
Your assignment of this week has two parts: programming and working with a paper.

I. Bag-of-words (5 points)

In this task you'll need to implement a BoW image classifier. For this,

1. Download STL-10 dataset from here https://cs.stanford.edu/~acoates/stl10/ (notice the link for the Python code to do the download). Only labeled part of the dataset will be used.

2. Repeat the steps of BoW algorithm using SIFT both as keypoint detector (not Harris affine detector) and descriptor. See here for help: https://docs.opencv.org/3.4/da/df5/tutorial_py_sift_intro.html . Please use k-means as clustering algorithm, for example as here https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html , and any classification algorithm on top, for example SVM ( https://scikit-learn.org/stable/modules/generated/sklearn.svm.LinearSVC.html#sklearn.svm.LinearSVC )

3. Evaluate your algorithm on the test set

4. Write conclusions for your work. Conclusions should be well-read and clear even for a person that did not see the previous points of the assignment done

II. Working with a source (2 points)

Look through the following paper https://www.researchgate.net/publication/220875352_Generic_Visual_Categorization_Using_Weak_Geometry . It was proposed by the same authors as BoW for image classification 2 years later. Your goal is not to read the paper in depth, but rather to understand the main ideas of it

What are the main differences with the original BoW approach? (2 points)

---

## Assignment 3

Your assignment this week will constitute of 2 parts, practical and theoretical.

Practical assignment: transfer learning for the task of image classification

- Using any (DL) classification model, e.g. ResNet, EfficientNet, ViT train on the dataset from your previous assignment. Taking into account the small (for DL) size of the dataset, use the pre-trained weights, freeze the bottom layers (responsible for feature extraction), and train only the top layers → 4 points

- Bonus task: retrain from scratch: re-initialize the weights and train the total of the network. Compare with the previous training. Write down your observations. → 2 points

**Theoretical assignment**

1. Take a look at this [paper](https://arxiv.org/pdf/2108.08810.pdf) making a study on the difference between CNN and ViT models. 

2. What are the questions being studied? → 1 point

3. How are the networks compared? (what is the methodology) → 2 points

4. What are the conclusions of the paper? → 1 point

---
## Assignment 5

This week you will work to compare the ground truth and the object detector output. In particular, you are asked to:

1. Calculate mAP (5 points)

2. Build precision-recall graph per class (2 points)

3. Build precision and recall as functions of threshold graphs (per class) (1+1 point)

---
## Assignment 6.1
This week you’ll get some labeling experience. For this, please:

1. Take 24 pictures of your hand

2. The hand should be showing 0 (fist) to 5 (open hand) fingers 

3. Segment the images using [labeler](https://www.robots.ox.ac.uk/~vgg/software/via/)

4. Add also number of fingers as a classification label

---
## Assignment 6.2

This week you’ll continue working with the hand dataset:

1. Combine your hand datasets

2. Do the cross-verification of labels (by importing labels in the labeler)

3. Do the data augmentation on this dataset (preserving the labels). Make a small report explaining the data augmentation type you have applied, with illustrations. Use external libraries if needed. 

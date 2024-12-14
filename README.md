# KERNELIZED PEGASOS-MULTICLASS CLASSIFICATION OF HANDWRITTEN DIGITS

This project describes the implementation of **Pegasos algorithm with Gaussian
kernels**, with the aim of training 10 binary classifiers for the multiclass classification of handwritten
digits. The dataset is retrieved from the online community Kaggle.

The **noise, time and space complexity** of the algorithm are **reduced** by using a **sample** from
the original dataset and the **principal component analysis (PCA)**.

The key concepts behind the implementation are:
- Support Vector Machine (SVM) algorithm
- Kernels
- one-vs-all encoding

There is an analysis of the cross-validated risk estimates for different values of **T
(the number of epochs)** and **λ (the regularization parameter)** reported on a **heatmap**. In this
analysis the parameter **gamma of the Gaussian kernel** is kept **constant**.

Another heatmap representing cross-validated risk estimates is plotted to illustrate the
performance of the algorithm for different values of the **regularization parameter** and the
**hyperparameter gamma** of the **Gaussian kernel**.

There is also an analysis of the impact on the Kernelized Pegasos performance by using different
types of kernels: **linear kernels, polynomial kernels,** and **Gaussian kernels**.

At the end, it is demonstrated that the use of PCA with 30 components leads to a
better complexity-performance trade-off compared to the algorithm used without PCA.

# Two-dimensional-PCA-for-Face-Image-Representation
## Introduction
  Principal component analysis (PCA) is a widely used technique for feature extraction, data representation, and pattern recognition. In the classical PCA, the 2D image matrices (i.e. m×n) must be initially converted to 1D vectors (R ^mn), usually resulting in a high dimensional image vector space. Consequently, there are difficulties to evaluate the covariance matrix (mn× mn) accurately when the matrix has large size and the number of the training samples is relatively small. Furthermore, computing the eigenvectors of a large size covariance matrix is time-consuming. Yang et al. (2004) developed the two-dimensional PCA (2DPCA) approach, which is based on 2D matrices rather than 1D vectors and directly computes eigenvectors of the so-called image covariance matrix (n×n). Because the size of the image covariance matrix of 2DPCA is significantly smaller than that of the corresponding covariance matrix of PCA, 2DPCA improves the accuracy and efficiency when evaluating the image covariance matrix and computing the corresponding eigenvectors, respectively.
In this project, the idea of the 2DPCA method and its algorithm will be reviewed in great detail, followed by the description of the 2DPCA-based image reconstruction. Furthermore, some experiments on a set of face images taken from the Yale Face Database (http://vision.ucsd.edu/content/yale-face-database) will be performed. Finally, some conclusions will be drawn, and future work will be proposed.

## Experiment and analysis
  The 2DPCA method was used for face reconstruction on the Yale database, which
contains 165 images of 15 subjects. And each person has 11 different images with varied facial
expressions and illumination and each image has the size of 243 by 320. In this report, the 11
different images of the subject 15 are chosen as the sample images (Figure 1) and the
reconstruction work is performed on the 3rd image (expression and illumination are both normal)
of subject 15 (Figure 2). The implementation of the 2DPCA algorithm and the following analysis
and visualization work were all performed by the python jupyter notebook. In particular, numpy
(https://numpy.org/) was used for matrix operation and matplotlib (https://matplotlib.org/) was
used for visualization.

## How to run the script
   run `Two-dimensional PCA project.ipynb`

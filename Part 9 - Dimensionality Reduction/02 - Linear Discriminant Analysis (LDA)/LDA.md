# Linear Discriminant Analysis - LDA
- Used as a dimensionality reduction technique
- Used in the pre-processing step for pattern classification
- Has the goal to project a dataset onto a lower-dimensional space

LDA is difference from PCA because in addition to finding the component axises with LDA we are interested in the axes that maximize the separation between multiple classes.

Breaking it down further:
- The goal of LDA is to project a feature space (a dataset n-dimensional samples) onto a small subspace subspace k(where $k \le n - 1$) while maintaining the class-discriminatory information.
- Both PCA and LDA are linear transformation techniques used for dimensional reduction. PCA is described as unsupervised but LDA is supervised because of the relation to the dependent variable.
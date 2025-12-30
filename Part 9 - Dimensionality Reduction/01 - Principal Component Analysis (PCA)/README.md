# Principal Component Analysis - PCA

**Used for:**
- Noise filtering
- Visualization
- Feature Extraction
- Stock market predictions
- Gene data analysis

**Goals:**
- Identify patterns in data
- Detect the correlation between variables
- Reduce the dimensions of a d-dimensional dataset by projecting it onto a (k)-dimensional subspace (where k<d)

**Overall Breakdown:**
- Standardize the data
- Obtain the Eigenvectors and Eigenvalues from the covariance matrix or correlation matrix, or perform Sigular Vector Decomposition.
- Sort eigenvalues in descending order and choose the $k$ is the number of dimensions of the new feature subspace ($k \le d$).
- Construct the projection matrix **W** from the selected $k$ eigenvectors.
- Transform the original dataset **X** via **W** to obtain a $k$-dimensional feature subspace **Y**
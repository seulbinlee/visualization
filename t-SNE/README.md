# t-SNE
### What is t-SNE
t-Distributed Stochastic Neighbor Embedding (t-SNE) is a nonlinear dimensionality-reduction algorithm designed for **visualizing high-dimension data** in a lower-dimensional space(typically 2D or 3D)

It converts similarities between data points into **probabilities** and tries to preserve these local relationships when projecting the data to a smaller space

### Key Ideas 
* Local structure preservation: Points that are close in the original space remain close in the lower-dimensional embedding
* Probabilistic mapping: Distances are modeled as probabilities using Gaussian distributions in the high-dimensional space and Student-t distributions in the low-dimension space
* Nonlinear projection: Unlike PCA (which is linear), t-SNE captures complex, nonlinear relationships between features
---
### `fit_transform(X, y=None)`
Fit `X` into an embedded space and return that transformed output
**Parameters**
* X : {array-like, sparse matrix} of shape {n_samples, n_features} or {n_samples, n_samples}
* y: None


**Returns**
* X_new : ndarray of shape (n_samples, n_components) - Embedding of the training data in the low-dimensional space

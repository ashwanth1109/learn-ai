# PRINCIPLE COMPONENT ANALYSIS

This is a tool used in machine learning, also called PCA. When working with machine learning, we usually deal with extremely large datasets that needs to be processed. So, we need reduction techniques to process this data.

PCA is a dimensionality reduction technique to reduce a larger set to a smaller one.

![PCA Dataset](https://raw.githubusercontent.com/ashwanth1109/learn-ai/master/UD104%20-%20Eigenvalues%20and%20Eigenvectors/PCA-Dataset.png)

From the sample 2D gaussian distribution we can see that the two variables are not independant. This is verified by the presence of the angled elliptical pattern.

Once we have the dataset, we calculate its corresponding covariance matrix.

```
[Va    Ca,b]
[Ca,b    Vb]
```

A covariance matrix is a symmetric matrix that expresses how the two variables relate to each other.

![PCA Dimension Reduction](https://raw.githubusercontent.com/ashwanth1109/learn-ai/master/UD104%20-%20Eigenvalues%20and%20Eigenvectors/PCA-Dimension-Reduction.png)

We try to find a new axis for the data, so that we can represent each data point in the set that has an (x,y) value to a one dimensional scalar value (r).
This value is the projection of the data point onto our axis.

To do this, we need to calculate the Eigenvalues and Eigenvectors of the covariance matrix.

![PCA Eigenvectors](https://raw.githubusercontent.com/ashwanth1109/learn-ai/master/UD104%20-%20Eigenvalues%20and%20Eigenvectors/PCA-Eigenvectors.png)

A 2 by 2 covariance matrix has two Eigenvectors (with two corresponding Eigenvalues) as illustrated above. We will select one of these two Eigenvectors as our axis for dimensional reduction. Our selection will be the one pointing in the direction of the larger spread since that's where most of the information is. In this case, it will be the longer arrow on the elliptical pattern.

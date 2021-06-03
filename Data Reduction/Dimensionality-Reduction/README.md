# Dimensionality Reduction
## Principal Components Analysis (PCA)
* Transforming the data to a new basis where the dimensions have low covariance and high variance.
   * Let X be the original matrix consisting the m data points as rows ( standarlize the data) and let P be the orthogonal matrix whose columns are linearly independent orthonormal vectors. hat{X} = XP is the matrix of transformed points. 
   * Covariance matrix (S) = (1 / m)X^TX, covariance matrix of the transformed data is P^TSP ( should be a diagonal matix for low covariance and high variance )
   * By Eigen value decomposition, P (new basis) whose columns are the eigen vectors of S will diagonalize S (X^TX).
* We select only the top k dimensions ( k eigenvectors or principal components ) along which the variance is high. (To get rid of noise and redundant dimensions)
   * The k value could be computed using the expected variance ratio.
   * The top k dimensions are the eigenvectors with higher eigenvalues ( eigenvalues correlates with variance ).   
* Applied to the Iris Dataset
    
## Reduct computation  

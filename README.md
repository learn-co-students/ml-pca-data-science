# ml-pca

Introduction
- What? Unsupervised learning: no labels/classes 
- Why?  dimensionality reduction, create new variables that are linear combinations of existing variables
- Before we start: standardize the data!!

Matrices and the eigendecomposition 
- Idea: start with computing the covariance matrix of your variables
- Decompose the matrix var(X) such that var(e’X) = e’ var(X) e is maximized
- Using lagrange function, it can be shown that L= e’ var(X) e, with L the eigenvalue and e the corresponding eigenvector.
- There are as many principal components (PC’s) as variables and
      - PC_j; j=1,...,p corresponding with X_1, X_2,...,X_p
      - PC_j = e_{j1}X_1+ e_{j2}X_2,...,e_{jp}X_p
      - var(PC_j)= L_j
- “PC score” is the value of a new variable for each observation: PC_j = e_{j1}X_1+...,e_{jp}X_p)

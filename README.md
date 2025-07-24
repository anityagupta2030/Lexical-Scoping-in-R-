# Lexical-Scoping-in-R-
#Assignment: Caching the Inverse of a Matrix #Matrix inversion is usually a costly computation and there may be some benefit to caching the inverse of a matrix rather than compute it #repeatedly (there are also alternatives to matrix inversion that we will not discuss here). My assignment is to write a pair of #functions that cache the inverse of a matrix.

#Write the following functions: #makeCacheMatrix: This function creates a special "matrix" object that can cache its inverse. #cacheSolve: This function computes the inverse of the special "matrix" returned by makeCacheMatrix above. If the inverse has already #been calculated (and the matrix has not changed), then the cachesolve should retrieve the inverse from the cache.

#Two Functions #Given a invertible matrix, the following two functions will calculate the inverse matrix or retrieve the inverse matrix from the cache.

#Function “makeCacheMatrix” creates a special “matrix” object that can cache its inverse. makeCacheMatrix contains 4 functions: set, get, #setmean, getmean. #(1)get is a function that returns the vector x stored in the main function. #(2)set is a function that changes the vector stored in the main function. #(3)setmean and getmean are functions very similar to set and get. #(4)They don’t calculate the mean, they simply store the value of the input in a variable m. #(5)into the main function makeVector (setmean) and return it (getmean).

makeCacheMatrix <- function(x = matrix()) {

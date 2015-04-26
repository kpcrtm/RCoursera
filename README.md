# RCoursera
Repository for R programming course on Coursera.  

The file cache.R contains the functions to demonstrate how to cache a matrix inverse into another environment so
that it can be fetched instead of being computed repeatedly in subsequent calls.  cache.R contains the following functions:


# Computes the matrix inverse or returns the version cached in 
# another environment
cacheSolve <- function(x, ...)

# Create a special matrix object that can be cached.  The <<- operation is 
# used to assign the object to another environment.
makeCacheMatrix <- function(x = matrix())

# This creates a 1000 x 1000 matrix and calculates the time to both
# calculate the matrix inverse and to fetch it from the cache
testCache <- function() 



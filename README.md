# RCoursera
Repository for R programming course on Coursera.  

The file inverseCache.R contains the functions to demonstrate how to cache a matrix inverse into another environment.  By caching the matrix inverse, R applications which require repeated use of the matrix inverse will run much faster.

The **testCache()** function demonsrates how to compute and cache the matrix inverse.

# inverseCache.R functions    
      
    makeCacheMatrix <- function(x = matrix())

Creates a special matrix object that can be cached in another environment.  The <<- operation is used to assign the object to another environment.
    
    
    cacheSolve <- function(x, ...)
    
Computes the matrix inverse or returns the version cached in 
another environment
    
    
    testCache <- function()
    
This creates a 1000 x 1000 invertable matrix and calculates the time to both
calculate the matrix inverse and to fetch it from the cache

# To run the test
&gt; source("inverseCache.R")      
&gt; testCache()

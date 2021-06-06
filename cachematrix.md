makeVector <- function(x = numeric()) 
  {
   inv <- null
    set <- function(y){
    x <<- null 
      
    }
    get <- function(){x}
    setInverse <-function(inverse)
    {
      inv  <<-inverse
    }
    getInverse <-function(){inv}
    
    list(set=set,get=get,setInverse=setInverse,getInverse=getInverse)
}
cachesolve <- fnction(x...){
  inv <-x$getInverse()
  
  if(!is.null(inv)){
    
    message("getting cache data");
    return(inv)
  }
  
  mat <-x$get()
  inv <-solve(ma.....)
  x$setInverse(inv)
  inv
  }

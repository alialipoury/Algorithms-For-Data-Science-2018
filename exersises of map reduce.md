# exersise2.3.1
## _(a)_   
### map function:
for each integer (k);produce (1 , k )
### reduce function:
for each (1 , k) from map we have the key 1 and associated values ; reduce function's task is producing (1 , max[k<sub>i ])

## _(b)_
### map function:
    for each integer (k);produce (1 , k )
### reduce function:
for each (1 , k) from map we have the key 1 and associated values ; reduce function's task is producing (1 , avg[k<sub>i ])
    
## _(c)_    
### map function:
for each integer (k);produce (k , k )
### reduce function:
for each (k , k) from map we have the key k and associated values([k<sub>i   ]) ; reduce  function's task is producing(k , 1) 

## _(d)_    
### map function:
for each integer (k);produce (k , k )
### reduce function:
for each (k , k) from map we have the key k and associated values([k<sub>i   ]) ; reduce  function's task is producing(k , 1)
    
### second map function:
for each (k , 1) from first reduce ; produce (1 , (k , 1))
###  second reduce function:
 produce (1 , (0 , sum(1,1 ,...)))
 
 
 # exercise2.3.2
 the solution had been written in the book for a square matrix makes sense for a r*c matrix .
 
  # exercise2.3.3
  ## _(a)_
  ### map function:
  for each tuple t in R and S emit key-value pair(t,1)
  ### reduce function:
  for each (t ,1) ; produce (t , sum(1,1,1,...))
  ## _(b)_
   ### map function:
 for each tuple t in R  emit key-value triple((R,t),1)) and likewise for  each tuple t in S  emit key-value triple((S,t),1))
  ### reduce function:
  for each triple in  R release (R , (t , sum(1,1,...))) likewise for S
   ### second map function:
   input triples from above reduce and map(R , (t , sum(1,1,...))) to (t , sum(1 ,1,1))  likewise for S
   ### second reduce function:
   now we have the (t)keys  and  a list of values like(t , sum());  release(t, min(sums))
   ## _(c)_
   ### map function:
  for each tuple t in R  emit key-value triple((R,t),1)) and likewise for  each tuple t in S  emit key-value triple((S,t),1))
  ### reduce function:
  for each triple in  R release (R , (t , sum(1,1,...))) likewise for S
  assume that sum(1,1,1) in R=r and in S=s
   ### second map function:
   input triples from above reduce and map(R , (t ,r)) to (t , r)  likewise for S
   ### second reduce function:
  release (t,k=r-s)
  
   ### third map function:
   input triples above and map identically
   ### third reduce function:
   if k>0 then produce k tuples of t else end
  # exercise2.3.4
  
  
    

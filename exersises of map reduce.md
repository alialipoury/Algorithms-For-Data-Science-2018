#exersise2.3.1
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
    

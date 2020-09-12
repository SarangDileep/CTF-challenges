# schush 

Rewrite the func as follows:

 x**12 + (x & (2**(bits/2)-1))
 ┆                                                                                                                                                                  
 x % 2^n == x & (2^n - 1) implies x**12 + x % 2^bits                                                                                                            
                                                                                                                                                                   
 ie, p=(x1^12)^1/2+x1%2^bits
 
 q=x2^12+x2%2^bits
 
 approx p=(x1^12)^1/2 
 
 q=x2^12                                                                                                                                                 
 
 ie, n=(x1^12)*x2^12 => n=((x1)*x2)^12                                                                                                                          
 
 ie,root(n,12)==x1*x2  
 
 now use factordb to find x1 and x2 and use these to find p and q
 
 finally solve using schmidt samao
 

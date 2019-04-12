# implement List.indexOf

2.
  a) y=log2x means that 2^y=x
  b) the graph is a curve that increases as x reaches infinity and slowly decreases as x reaches 0. The curve never crosses the y-axis, but it crosses the x-axis at (1,0).

3)
  0. Given a sorted list of length n, find the index of a given value
  1. Given a sorted list of length n/2, find the index of a given value
  2. 
    a) Boolean: check if the list is out of values, in our case we use low is greater than high.
    b) Base Case Solution: return -2 to show the value is non-existant
    c) Recursive cases solution:
          
          int pageToCheck = (low + hi) / 2;
          int comparison =
            findMe.compareTo( list_iAS.get( pageToCheck));

          if( comparison == 0)   
              return pageToCheck; 
  
   d) Recursive abstraction:
   
          return indexOf_recursive( findMe
                                           , low
                                           , pageToCheck -1);

          return indexOf_recursive( findMe
                                          , pageToCheck +1
                                          , hi);

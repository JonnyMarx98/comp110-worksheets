a) This algorithm checks if there is a duplicate in the list. It does this by starting with the first item in the list and checking, in order, every other item in the list to see if they match. It then does this with the second item. When it finds a duplicate it returns true. 

B)  Because there are is a for loop within a for loop (a nested loop). This means in the worst case the algorithm will have to check through n*n times to find the duplicate.  

C) It is still correct because every value of j is still checked with every value of I.  

D) The algorithm will run twice as fast because it will not check the same list index's twice like the original algorithm would. For example  in the original algorithm, if I = 5 and j = 4 it would check if list[5] = list[4] which is the same as if I = 4 and j= 5.  

E) No its not quadratic because it no longer has to check the through n*n times.  

F) O(N Log N) [1]  

G) O(N^2 Log N) The time complexity of the sort function is O(N Log N) and the time complexity of the for loop is O(N), so multiplying these together you get O(N^2 Log N) 

H) As n increases n^2 log n will eventually grow larger than n^2 so for larger values the first algorithm, with time complexity O(N^2) will run faster.  

I) Because it will be faster for short lists.

[1](https://www.ics.uci.edu/~pattis/ICS-33/lectures/complexitypython.txt)

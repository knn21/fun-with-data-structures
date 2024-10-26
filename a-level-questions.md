# Theory
## 2022 A Level P1 Q4
*Solution:*

(a) advantages of using fixed capacity array over linked list to store ordered items
- constant time O(1) access to smallest (first index) and largest (last index) items 
- logarithmic time O(lg n) binary search access as data is sorted 

(b) advantages of using linked list over fixed capacity array to store ordered items
- constant time O(1) access to insert smallest item to head of linked list
- efficient use of memory to insert item into correct position by adjusting pointers

(c)(i) recursive

(ii) base/terminating case

(iii) computes size of linked list / number of items in linked list recursively

(d)

```
FUNCTION Z(Head)
    IF Head is NIL OR Head.next is NIL
        RETURN Head
    ENDIF
    newHead = Z(Head.next)
    Head.next.next = Head
    Head.next = null    
    RETURN newHead
ENDFUNCTION
```
(e) why mergesort may be faster than quicksort in this situation
- mergesort is a divide and conquer algorithm and for any data set (ordered or unordered) is guaranteed to perform in O(n lg n) linearithmic efficiency as the split phase will evenly divide the array by half achieving O(lg n) performance
- quicksort will not perform well for an ordered data set if the pivot is chosen to be the first (smallest) or last (largest) item, as this will unevenly divide the left and right subarrays (effectively reducing the problem size only by one item instead of half the number of items) leading to worst case O(n^2) quadratic time complexity.

## 2022 A Level P1 Q8
*Solution:*

## 2021 A Level P1 Q4
*Solution:*

## 2021 A Level P1 Q5
*Solution:*

## 2021 A Level P1 Q7
*Solution:*

## 2020 A Level P1 Q3
*Solution:*

a) (https://github.com/user-attachments/assets/0be35e78-5959-4893-be88-cc32dc8157eb)

b) 0 or 2 or 4 or 6 (any 1)

c) 
(i) 
● Function that is defined in terms of itself. / calls itself during runtime 
● Calls itself with one or more similar but smaller subproblems.
● Repeats itself several times and with each recursive call, the problem is brought closer to the
base case.
● Once the terminating case/ base case is reached, it stops calling more functions. A base case or terminating case is the smallest problem that can be solved trivially.

(ii)  03, 06

(iii)  To check if a leaf node is reached 

d)  Trace Table 

Index | Output 
--------------
0     | A
--------------
2     | B
--------------
1     | +
--------------
4     | C
--------------
6     | D
--------------
5     | -
--------------
3     | *
--------------

e) 
● Call stack is used to keep track of recursive calls.
● When a recursive call is made, the return address at which the function is called and current contents of the local variables are stored on the stack as a stack frame.
● Each recursive call will push another stack frame to the stack until the base case is reached.
● Once the base case is reached, the main will return to the caller of the function by popping off the stack frame, restoring the return address and contents of the local variables of the caller.
● The process of popping off the stack frame will continue until the control is back to the first caller to the function.

f) postorder

g) Queue is a linear data structure that follows the First In First Out (FIFO) principle.
First element that is added to the queue is also the first one to be removed from the queue.
Queue preserves order of data

h)
- Circular queue has fixed size that can be reused but linear queue with fixed array implementation will keep decreasing in size due to previously dequeued memory locations 

 -Linear queue has fixed start and ending indexes but circular queue wraps around with tail connected back to the start
 
---
# Practical
## 2024 A Level P2 Task 2
- Tree
## 2022 A Level P2 Task 3
- BST
## 2021 A Level P2 Task 3
- Linked List, Queue

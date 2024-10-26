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

a) dynamic memory allocation is more flexible than static memory allocation. 
For static data structure, a fixed amount of memory is reserved for data even though less memory may be needed during runtime. For dynamic data structures, the person implementing the data structure can easily expand or contact the memory space as needed by the programme 

b) Problems of dynamic data struct
- inserting/ deleting will require memory allocation/ deallocation which may lead to longer runtimes or slower performance 
- dynamic data structures can potentially use up all of the memory on the system/ device causing programs that require memory to not work (contrasts with static memory allocation which only can use memory that has been allocated)

c) array
no chance of memory overflow 
availability of binary search as a way to look up entires within the system

## 2021 A Level P1 Q5
*Solution:*

## 2021 A Level P1 Q7
*Solution:*

## 2020 A Level P1 Q3
*Solution:*

---
# Practical
## 2024 A Level P2 Task 2
- Tree
## 2022 A Level P2 Task 3
- BST
## 2021 A Level P2 Task 3
- Linked List, Queue

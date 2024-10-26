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

a) 3 features of good hash algorithm
● Should use all parts of the input data.
● Generate very different hash values for a small change in the input data.
● Hash values it generates should be uniformly/ equally distributed across the entire range of possible hash values (minimise the number collisions).

b) 2 Methods choose 1
CLOSED ADDRESSING
If collision occurs, the data is not stored in the position it is hashed to.
Instead, another location is assigned for it to be inserted.
eg. Linear probing: record gets inserted into next adjacent cell
Quadratic probing: record gets inserted i**2 cells away (prevents clustering)

OPEN ADDRESSING
Collided data is always stored in the same position it is hashed to. Some other forms of data structure are usually used to store all the data
at the calculated position(bucket). Hence, the index in the bucket where the data
is stored should be located.
eg. LinkedList to store collided/overflow entries

c) Hash table search has average time complexity of O(1) with optimal hashing algorithm as it can directly access the location where data is located but linear search has average time complexity O(n) as it has to traverse/ iterate through the list to find the target element. hash table is more prefered than linear search to locate a record due to its increased efficiency 

d) Binary Search only works if dataset is sorted in order which may not true in this situation. If dataset is not sorted, efficiency of algorithm used to sort the dataset has to be accounted for making binary search disadvantageous 

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

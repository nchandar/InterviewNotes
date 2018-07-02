# LinkedList

## Linked list vs Arrays

| S.No  | Arrays                                       | Linked Lists            |
| :---: |:-------------                                | :--------------------   |
|   1   | Fixed Size                                   | Dynamic Size            |
|   2   | Inefficient insertion and deletion           | Efficient insertion and deletion |
|   3   | Random Accessing (i.e efficient indexing).   | No Random Accessing     |
|       | Eg. Can retrive a element randomly using the index value like a[5] to get the 6th element in the array. |                                              
|   4   | Results in memory waste due to declaring the size of the array upfront and if its not used| No memory waste.|
|   5   | Sequential Access is faster. Since elements are in contiguous Memory location.| Sequential Access is slow. Since elements are not in contigous memoru location.|


## Two types of Linked List
  1. Singly Linked List
  2. Doubly Linked List
  
### Singly Linked List

A linked list basically consists of multiple nodes and a node basically has Data and a pointer to the next element(node).
![Image1](https://github.com/nchandar/InterviewNotes/blob/master/Node.png)


![Image2](https://github.com/nchandar/InterviewNotes/blob/master/SinglyLinkedList.png)

<b>Head :- </b> The beginning of the chain is called the head. </br>
<b>Null :- </b> The end of the chain is indicated by a null.

  - <b>length Method</b> retrieves the number of nodes in a list.
  - <b>head Method</b> assigns a node as the head of a list.
  - <b>add(value) Method</b> adds a node to a list.
  - <b>searchNodeAt(position) Method</b> searches for a node at n-position in our list.
  - <b>remove(position) Method</b> removes a node from a list.

### Doubly Linked List
##### Advantages over singly linked list
1) A DLL can be traversed in both forward and backward direction.
2) The delete operation in DLL is more efficient if pointer to the node to be deleted is given.
3) We can quickly insert a new node before a given node.
In singly linked list, to delete a node, pointer to the previous node is needed. To get this previous node, sometimes the list is traversed. In DLL, we can get the previous node using previous pointer.

##### Disadvantages over singly linked list
1) Every node of DLL Require extra space for an previous pointer.
2) All operations require an extra pointer previous to be maintained. For example, in insertion, we need to modify previous pointers together with next pointers. For example in following functions for insertions at different positions, we need 1 or 2 extra steps to set previous pointer.

More Reference :- https://www.tutorialspoint.com/data_structures_algorithms/linked_list_algorithms.htm

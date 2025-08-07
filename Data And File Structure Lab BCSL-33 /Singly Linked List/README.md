C Program to Implement Singly Linked List

A linked list is a linear data structure used to store elements of 
the same data type but not in contiguous memory locations. 
It is a collection of nodes where each node contains a data 
field and a next pointer indicating the address of the next node. 
So only the current node in the list knows where the next element of the list is stored.

Implementation of Singly Linked List in C

A singly linked list is a type of linked list where only the address 
of the next node is stored in the current node along with the data 
field and the last node in the list contains NULL pointer. This makes 
it impossible to find the address of the particular node in the list 
without accessing the node previous to it. So we can only access the 
data sequentially in the node.


Algorithm

Insertion Operation Implementation

1. Algorithm for insertAtFirst Function

* Create a new node.
* If the linked list is empty set the new node as the Head  and return.
* Connect the next pointer of this new node to the Head of the linked list.
* Update the Head pointer and make it points to the new node

2. Algorithm for insertAtPosition Function

* If it is 0, call the insertAtFirst function to insert the node at the first position of the list.
* Check if the position is 0.
* Initialize a counter variable and a temporary pointer to traverse the linked list.
* Iterate over the linked list to find the node before the insertion point (position - 1).
    - If the temporary pointer becomes NULL before reaching the desired position, the position is out of range. Return.
* Create a new node.
* Point the next pointer of the new node to the node present just after the temporary pointer.
* Point the next pointer of the temporary node to the new node and return.


3. Algorithm for insertAtEnd Function

* Create a new Node.
* If the list is empty, update the Head pointer to be this new node and then return.
* Otherwise traverse till the last node of the singly linked list.
* Connect next pointer of the last node to the new node.


Deletion Operations in a Singly Liked List in C

1. Algorithm for deleteFromFirst Function

* Ensure that the Head of the linked list is not NULL; if it is, the list is empty, so return.
* Create a temporary pointer and point it to the current Head of the list.
* Update the current head of the singly linked list to the next node.
* Point the next pointer of the temporary node to NULL to detach it from the singly linked list.
* Delete the temporary node.


2. Algorithm for deleteFromPosition Function

* If it is NULL, the linked list is empty, so return.
* Check if the head pointer of the linked list is NULL.
* Check if the position is 0.
    If it is 0, call the deleteFromFirst function to delete the first node.
* Initialize a counter variable and a temporary pointer to traverse the linked list.
* Iterate the linked list to find the node before the deletion point (position - 1).
* If the temporary pointer becomes NULL before reaching the desired position the position is out of range. Return
* Store the next node of the temporary pointer in a temporary pointer.
* Update the next pointer of the temporary pointer to the next pointer of the node to be deleted.
* Delete the node represented by the temporary pointer.


3. Algorithm for deleteFromEnd Function

* Ensure that the Head of the linked list is not NULL; if it is, the list is empty, so return.
* If the singly linked list has only one node, delete the head node and point the head pointer to NULL.
* Traverse till the second last node of the singly linked list.
* Store the next node of the second last node in a temporary pointer.
* Connect the next pointer of the second last node to NULL.
* Delete the last node represented by the temporary pointer.


Algorithm for Print Function

* Check if the HEAD of the singly linked is is NULL or not. If NULL return back.
* Set a temp pointer to the head of the singly linked list.
* While temp pointer != NULL:
    - Print temp->data.
    - Move temp to temp->next
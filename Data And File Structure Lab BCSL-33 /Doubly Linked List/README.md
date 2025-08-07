Doubly Linked List in C

A doubly linked list is a type of linked list in which each node contains 3 parts, 
a data part and two addresses, one points to the previous node and one for the next node. 
It differs from the singly linked list as it has an extra pointer called previous that 
points to the previous node, allowing the traversal in both forward and backward directions.

Doubly Linked List Representation in C

A doubly linked list is represented in C as the pointer to the head (i.e. first node) in the list. 
Each node in a doubly linked list contains three components:

1. Data: data is the actual information stored in the node.
2. Next: next is a pointer that links to the next node in the list.
3. Prev: previous is a pointer that links to the previous node in the list.

Basic Operations on C Doubly Linked List

We can perform the following basic operations in a doubly-linked list:

* Insertion
* Deletion
* Traversal

1. Insertion in Doubly Linked List in C

Inserting a new node in a doubly linked list can be done in a similar way like inserting a new node in a singly linked list but we have to maintain the link of previous node also. We have three scenarios while inserting a node in a doubly linked list:

* Insertion at the beginning of the list.
* Insertion at the end of the list.
* Insertion in the middle of the list.


2. Deletion in a Doubly Linked List in C

Just like insertion, we have three scenarios while deleting a node in a doubly linked list:

* Deletion from the beginning of the list.
* Deletion from the end of the list.
* Deletion at specific position of the list.


3. Traversal in a Doubly Linked List in C

Traversal in a doubly linked list means visiting each node of the doubly linked list to perform some kind of operation like displaying the data stored in that node. Unlike singly linked list we can traverse in doubly linked list in both the directions.

* Forward Traversal: From head node to tail node
* Reverse Traversal: From tail node to head node
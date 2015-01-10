DATA STRUCTURES STUDY GUIDE:book::book::book:
===========================


Welcome to my CS 112 study guide. There are a few references to the textbook within the study guide so
be prepared to use it. There are also many links to videos to help you understand topics covered in 
the course. I try and choose videos that have the shortest and best explanations possible to make learning 
the course material as quick and easy as possible. The videos are helpful, but some concepts are difficult to
grasp and therefore the textbook is a gold mine of information for your full understanding of certain concepts.





Part I:  Linear Structures
=========================
:boom: Linear structures are the easiest part of CS 112, so make sure you take advantage of this and destroy the first exam and the first few assignments that use linear data structures. :boom:

1.) Linked Lists
---------------
Circular Linked Lists and doubly linked lists don’t usually appear on exams, but it is still good to learn them
to increase your understanding of linked lists in general.

:white_check_mark: Regular Linked Lists and Circular Linked Lists Summary [Sec 4.5 - 4.6] 
----------------------------------------------------------------------------

[Imagining a Linked List (Sesh Venugopal)](https://www.youtube.com/watch?v=_ri3Qm5A4Dk)
  - Definition (Linked List): Linear structure consisting of nodes. Each node contains a piece of data and a pointer that     points to the next node in the linked list.
  - Difference between linked list and array:

          Operation           |     Array                  | Linked List
          ------------------- | -------------------------- | ------------
          Access              |    Random                  | Sequential from beginning of list (in order)
          Insertion/Deletion  | entries have to be shifted |Nothing must be done to entries
          Storage             |Allocated in one shot (initial size of array cannot change)| Allocated only when needed (Initial size of list can change)

  
- Generic definition of a node (look at [Generic Types](https://github.com/RUSpaceCadet/DATA-STRUCTURES/blob/master/STUDYGUIDE.md#3-generic-types) to fully understand image below):

  ![Alt text](https://github.com/RUSpaceCadet/DATA-STRUCTURES/blob/master/STUDYGUDIE%20IMAGES/GENERIC%20NODE.PNG "Generic node definition image")
  

###### - Insertion of a node in LL
-----------------------------------

  A node can be added to the front of the linked list, the end of the linked lists or in between two different   nodes

  |CASE 1 Adding a node to the front of an LL|
  --------------------------------------------

  1.) Create node to be added

  2.) Make the new node point to the first node in the linked list

  3.) Make first node point back to new node.

  Example Code:
  
  Assuming first node in LL is called 'front'.

  ![Alt text](URL "2 Adding to front of LL")

  There is an even simpler way to add a node to the beginning of the LL:

  ![Alt text](URL "3 Adding to front of LL (Simplified)")

  CASE 2: Adding a node to the end of a LL:

  1.) Create node to be added

  2.) Make last node point to the new node.

  3.) Make new node point back to last node.

  Example Code:

  Assuming last node in LL is called 'last'.
  
  ![Alt text](URL "4 Adding to end of LL")

  CASE 3: Adding node in between two nodes (Most probably the most complicated):

  Assume newnode is being added after a node called 'v'.

  1.) Create node to be added

  2.) Make new node point to node in front of 'v'.

  3.) Make 'v' point to new node.

  Example code:  

  ![Alt text](URL "5 Adding in between two nodes")


- Deletion of a node in LL
  
  There are three basic deletion situations: deleting node from the front of LL, end of LL and in between two nodes in the LL.

  CASE 1: Deleting from front of LL:

  Assuming the first node in an LL is called 'front'.

  Deleting the first node in an LL is  a special case and takes only one step:

  1.)Make the node after front be equal to front.

  Example code:

  ![Alt text](URL "6 Deleting from front of LL")

  CASE 2: Deleting node in between two nodes in LL:

  Assuming the node 'v' is in front of node to be deleted.

  1.) Make reference to node to be deleted (oldnode)

  2.) Delink oldnode by making v point to node in front of oldnode.

  Example code:
  
  ![Alt text](URL "7 deleting node from in between two nodes")

  CASE 3: Deleting from end of LL:

  Deleting from the end of an LL is similar to deleting a node in between two nodes.
  The same code that we used in CASE 2 can be used here as the only difference would be oldnode.next being equal to null.

  SPECIAL CASE: Deleting only node in LL:

  Assuming the only list in node is called front.

  1.)Set front to null.

  Example code:

  ![Alt text](URL "8 deleting only node in LL")


- Traversing through LL

  Traversing through an LL is useful for when you would like to print out all entries in the LL, find a specific location in the LL where you would like to insert an item or find a specific node that you would like to delete.

  Assuming the first node in the LL we would like to traverse is called front, we can use any type of loop to print the information held within all the nodes in the LL.

  Examples:

  Using for loop:

  ![Alt text](URL "9 Traversal with for loop")

  Using While Loop:

  ![Alt text](URL "10 Traversal using while loop")

  
  Video for further explanation on implementation of LL in Java: [Regular Linked List in Java (Derek Banas)](https://www.youtube.com/watch?v=195KUinjBpU)


  Circular Linked List:
  - Definition (Circular): Normal linked lists in which the last node refers back to the first.

  - Insertion of a node in CLL

   CASE 1: Inserting in between two nodes in a CLL is the same process as in a regular LL.

   CASE 2 & 3: Inserting at the beginning and at the end of an CLL is the same process as the last node refers back to the first node.

   Assuming the node pointing to the first node is called 'last'.

   1.) Create new node

   2.) Check if CLL is empty (Code will give a null pointer exception if list is 
   empty)

   3.) Link new node to first node
   
   4.) Link last node to new node

   Example Code:

   ![Alt text](URL "11 Insertion CLL")

   - Deletion of a node in CLL


###### :white_check_mark: Doubly Linked List 
--------------------------------------------
 [Introduction to Doubly Linked List ](https://www.youtube.com/watch?v=JdQeNxWCguQ) [Programming Problems P4.14, P4.16]

2.) Exceptions [1.5]
--------------------

3.) Generic Types
------------------

4.) ArrayList
--------------

5.) Complexity Order/Running Time and Space
-------------------------------------------

6.) Stack
----------

7.) Queue
---------


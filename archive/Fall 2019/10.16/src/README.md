# Linked Lists and the List Interface

### Previously, on CSC 143

**Linked Lists** are a type of data structure that stores a sequence of elements chained together using references (pointers).

Unlike the ArrayList, which uses an Array as a backing container to store elements contiguously and has `O(1)` indexing,
the Linked List has `O(n)` indexing as the list must be traversed.

However, the Linked List has the advantage of `O(1)` insertion and deletion,
whereas the ArrayList has `O(n)` insertion and deletion due to the need to shift elements.

A Linked List is composed of several "node" instances for every element in the list, storing a value and pointer to the next element.

We can *abstract* away the complexity of node management by writing a Linked List class which manages nodes,
and exposes easy-to-use public methods like `size()` that mask the underlying implementation.

A consequence of *abstraction* is that runtime and memory cost of operations are hidden to the client.
As an engineer, the choice of data structure used can have a significant impact on the performance of your program. 

## Linked List Algorithms

Linked Lists are provide several interesting algorithmic opportunities, which are implemented
quite differently than with ArrayLists.

These problems are also commonly found as technical interview questions! Let's write some of them together.

See: LinkedList.java

## Stack

A *stack* is a data structure which mimics a stack of items in real life. It supports operations:

 - Push, that inserts an element on the top of the stack
 - Pop, that returns and removes the element on top of the stack
 - Peek, which returns the element on top of the stack

Whiteboard: Linked List as Stack

## Queue

A *queue* is a data structure which mimics a queue in real life. It supports operations:

 - Add (enqueue), that inserts an element to the back of the queue
 - Remove (dequeue), returns and removes an element in the front of the queue
 - Peek, which returns the element in front of the queue
 
Whiteboard: Linked List as Queue

## Doubly Linked Lists

The *Doubly* Linked List extends the *Singly* Linked List by adding a reference to the previous node
for each node in the list.

See: DoubleNode.java

Whiteboard: Doubly Linked Lists

See: Project 2

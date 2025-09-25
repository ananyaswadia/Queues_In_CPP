# Queues_In_CPP
## Aim
To study and implement Quese data structure in C++
## Theory
Queue container follows the FIFO (First In First Out) order of insertion and deletion. According to it, the elements that are inserted first should be removed first. This is possible by inserting elements at one end (called back) and deleting them from the other end (called front) of the data structure.

### Basic Operations
1. Inserting Elements-New elements can only be inserted at back of the queue using push() function. The process of inserting elements in a queue is also called enqueue.

2. Accessing Elements-Only the front and back elements of the queue can be accessed by using front() and back() functions respectively.

3. Deleting Elements-Elements can only be deleted from the front of the queue using the pop() function. This operation is also called dequeue.

4. empty()-This checks whether the queue is empty. It returns true if the queue has no elements; otherwise, it returns false.

5. Size of queue-The size() function in a queue returns the number of elements currently in the queue. It helps to determine how many items are stored without modifying the queue.


<img width="1082" height="384" alt="image" src="https://github.com/user-attachments/assets/c79e89d3-075e-44ba-b31e-31c950acf859" />


## Algorithm
### Initialization
1. Define a constant SIZE = 5 for the maximum size of the queue.

2. Create a class Queue with:

3. An integer array arr[SIZE] to store queue elements.

4. Two integer variables front and rear to track the front and rear of the queue.

5. In the constructor: Set front = -1 and rear = -1 to indicate an empty queue.
## Enqueue Operation (Insert Element)
1. Input: An integer value to insert.

2. Steps: Check if rear == SIZE - 1: If true, print "Queue Overflow!" and exit. If front == -1, set front = 0 (first insertion).

3. Increment rear and insert value at arr[rear].

4. Print that the value was inserted.
### Dequeue Operation (Remove Element)
1. Steps: Check if front == -1 or front > rear:
2. If true, print "Queue Overflow!" (actually underflow) and exit.
3. Print the value at arr[front] as removed.
4. Increment front.
### Display Operation
1. Steps: Check if front == -1 or front > rear:
2. If true, print "Queue is empty." and exit.
3. Loop from front to rear and print each element.
### Main Function Execution
1. Create a Queue object q.
2. Perform the following operations:
3. q.enqueue(10) , q.enqueue(20) , q.enqueue(30) , q.display() → Shows 10, 20, 30
4. q.dequeue() → Removes 10 , q.display() → Shows 20, 30 , q.enqueue(40)
5. q.display() → Shows 20, 30, 40
## Conclsion
We learnt to perform baic operations on queues like adding and removing elements.

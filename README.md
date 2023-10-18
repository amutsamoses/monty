0x19. C - Stacks, Queues - LIFO, FIFO

Alx Team project:
AUTHORS;
	Kephar Moses <amutsamoses@gmail.com>
	Dinka Wolde  <dinkawolde09@gmail.com>

Data Structure and Algorithm in C
Topic: STACK & QUEUES

1. STACK
A stack is a linear data structure, a collection of items of the same type.
In a stack, the insertion and deletion of elements happen only at one endpoint. The behavior of a stack is described as “Last In, First Out” (LIFO). When an element is “pushed” onto the stack, it becomes the first item that will be “popped” out of the stack. In order to reach the oldest entered item, you must pop all the previous items.

Operations Performed on StackS: 

push: Adds an element to the top of the stack.
pop: Removes the topmost element from the stack.
isEmpty: Checks whether the stack is empty.
isFull: Checks whether the stack is full.
top: Displays the topmost element of the stack.

Underlying Mechanics of Stacks
Initially, a pointer (top) is set to keep the track of the topmost item in the stack. The stack is initialized to -1.
Then, a check is performed to determine if the stack is empty by comparing top to -1.
As elements are added to the stack, the position of top is updated.
As soon as elements are popped or deleted, the topmost element is removed and the position of top is updated.

Implementing Stack in C
Stacks can be represented using structures, pointers, arrays, or linked lists.

Time Complexity of Stack Operations
Only a single element can be accessed at a time in stacks.
While performing push() and pop() operations on the stack, it takes O(1) time.

2. QUEUES
A queue in C is basically a linear data structure to store and manipulate the data elements. It follows the order of First In First Out (FIFO).
In queues, the first element entered into the array is the first element to be removed from the array
A queue is open at both ends. One end is provided for the insertion of data and the other end for the deletion of data.
A queue can be implemented with any programming language such as C, Java, Python, etc.

Operations Associated with a Queue in C
isEmpty(): To check if the queue is empty
isFull(): To check whether the queue is full or not
dequeue(): Removes the element from the frontal side of the queue
enqueue(): It inserts elements to the end of the queue
Front: Pointer element responsible for fetching the first element from the queue
Rear: Pointer element responsible for fetching the last element from the queue

Working of Queue Data Structure
Queue follows the First-In-First-Out pattern. The first element is the first to be pulled out from the list of elements.
Front and Rear pointers keep the record of the first and last element in the queue.
At first, we need to initialize the queue by setting Front = -1 and Rear = -1
In order to insert the element (enqueue), we need to check whether the queue is already full i.e. check the condition for Overflow. If the queue is not full, we’ll have to increment the value of the Rear index by 1 and place the element at the position of the Rear pointer variable. When we get to insert the first element in the queue, we need to set the value of Front to 0.
In order to remove the element (dequeue) from the queue, we need to check whether the queue is already empty i.e. check the condition for Underflow. If the queue is not empty, we’ll have to remove and return the elementat the position of the Front pointer, and then increment the Front index value by 1. When we get to remove the last element from the queue, we will have to set the values of the Front and Rear index to -1.

Implementation of Queue in C
Queues in C can be implemented using Arrays, Lists, Structures

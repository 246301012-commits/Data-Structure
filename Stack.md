Stack is the linear data structure that follows the Last in, First Out(LIFO) principle of data insertion and deletion.
Think of it as the stack of plates stacked on top of one another where we can only add or remove the top plate.

**Representation of Stack in C**
The stack can be represented as a structure that contains a fixed-size array in C which stores the data of the stack and an index pointer which is used to track the top element of the stack.

struct stack {
     type arr[MAX_SIZE];
     int top;
}

**Basic Stack Operations in C**
Push -> Inserts an element at the top of the stack.
Pop -> Removes the top most element of the stack.
Peek -> Returns the topmost element of the stack.
IsFull -> Returns true is the stack is full otherwise returns false.
IsEmpty -> Returns true is the stack is empty otherwise returns false.


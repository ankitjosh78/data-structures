# Data Types
A data type defines a domain of allowed values and operations that can be performed on those values.

For example:

   __int__ data type can take values in a range and various operations can be performed on it such as addition, substraction, division, multiplication, etc.
   
These are all built-in data types. Other examples include __float__, __bool__, __char__ . The __operations and values for these data types are predefined in the language__. 
   
A brief overview of these common builtin data types:

1)float - used to store floating point numbers, can be negative as well as positive.

2)char - used to store a single character.

3)bool- used to store a logical result such as true(1) or false(0).

Now, to use a data type that is not defined in the language itself, it is the __programmer's responsibility to define it__ and __set the operations and the domain of values for it__.


## Abstract data types:

Abstract data type is a concept which defines a data type logically. It specifies a set of instructions for the values and operations. 

ADT tells us __what is to be done__ and __not how it will be done__ , or the algorithms used in it, or the representation of it in memory.

The user need not know how the data is implemented in memory. Example: We know about _int_, _float_ and can perform operations on them without knowing how they are actually implemented. 

So for an ADT , the user __needs to know what it can do__ and __not how it does it__. 

Example:

  __STACK__:
  
  A stack is defined a data structure which contains elements of same type and supports a bunch of specific operations, which are:
  
  0)initialize() - initializes the stack.
  1)push() - inserts an element at one end of the stack.
  2)pop() - removes and returns the topmost element of the stack at the same end.
  3)peek() - just returns the topmost element of the stack without removing it.
  4)size() - returns the number of elements in the stack.
  5)isEmpty() - returns true if there are no elements in the stack.
  6)isFull() - returns true if the stack has reached it's maximum limit.
        

We can see that over here, in the STACK data type , there are a __bunch of operations that are allowed__. But we __don't talk about how they are going to be implemented__. 

There can be __multiple ways to implement a ADT__.  
        
The __differences are mostly time and space efficiencies__.         
        


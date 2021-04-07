# What the heck is an array?
   Well, an array is just an __ordered  collection of similar types of data__ and each of those __data items in it is called an element of the array__. 
   
   Now, the datatype of the elements can be __any valid data type__ like _int_, _float_, _char_, _string_, _bool_.
   
   One thing to note is that: __the elements__ of an array share the __same variable name__ but has __different index__.
         
   ### Example:
   To store the weights of 10 of your friends, we can take an array named _wt_ of type _int_ and of size 10.
   
   In C/C++, it would look something like:
   
   _int wt_[10];  where each elements will be in order: _wt_[0],_wt_[1],....,_wt_[9]
   
   (Remember: The indexing starts from 0)
        Over here, _wt_[0] is the first element, _wt_[1] is the second element and so on.
    
  ### Now that you know what an array is, you need to know about the dimension of an array. 
    
  
  Arrays can be one dimensional as well as multidimensional. 
  
  __How to tell the dimension you may ask?__ 
  
  Well _"the number of subscripts"_ in an array determines it's dimension.
    
  In our example, we saw an one-dimensional array as it had only _one subscript_.
  
  A two dimensional array would be something like: __arrayName[][]__;
    
    
## One Dimensional Arrays:
   ### Declaration 
   Arrays can be declared like any other simple variables.
   
   __Syntax: _data_type_ array_name[size]__ 
   
   __Example: _int_ wt[10], _float_ height[20], _bool_ correct[20], where "wt", "height", "correct" are the array names.__ 
   
   So the syntax _float_ height[20] , means it is a floating value array and can store upto 20 such elements in it.
  
   __Points to keep in mind:__
   
   1) When an array is declared, the amount of space that is need to hold all the elements is allocated in the memory.
   2) The size of the array must be known during compilation time.
   3) We can't use any variables for specifying the size of the array. If it's a variable then it's value must be known.
  ### Accessing the elements:
  The elements in the array can be accessed by specifying the array name and the index in brackets. 
  
  Index 0 is known as the lower bound of the array and the last index is known as the upper bound of the array.
  
  So, for a integer array named "arr" of length 3, the elements would be arr[0], arr[1], arr[2]. 
  
  Over here, 0 is the lower bound and 2 is the upper bound.
  
  ### Processing
  To process an array, the most common way of doing it is to use a _for_ loop.
  
  The loop variable is used in place of the index of the array. It should start from 0 , because we want to access the whole array and should go on till the last index while incrementing by 1.
  
   __Example:__
   1) For reading:
   
     for(int i=0;i<3;i++)
        scanf("%d", &arr[i];
   2) For printing:
   
     for(int i=0;i<3;i++)
        printf("%d", arr[i];

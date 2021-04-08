# What the heck is an array?
   Well, an array is just an __ordered  collection of similar types of data__ and each of those __data items in it is called an element of the array__. 
   
   Now, the datatype of the elements can be __any valid data type__ like _int_, _float_, _char_, _string_, _bool_.
   
   One thing to note is that: __the elements__ of an array share the __same variable name__ but has __different index__.
         
   #### Example:
   To store the weights of 10 of your friends, we can take an array named _wt_ of type _int_ and of size 10.
   
   In C/C++, it would look something like:
   
   _int wt_[10];  where each elements will be in order: _wt_[0],_wt_[1],....,_wt_[9]
   
   (Remember: The indexing starts from 0)
        Over here, _wt_[0] is the first element, _wt_[1] is the second element and so on.
    
  #### Now that you know what an array is, you need to know about the dimension of an array. 
    
  
  Arrays can be one dimensional as well as multidimensional. 
  
  __How to tell the dimension you may ask?__ 
  
  Well _"the number of subscripts"_ in an array determines it's dimension.
    
  In our example, we saw an one-dimensional array as it had only _one subscript_.
  
  A two dimensional array would be something like: __arrayName[][]__;
    
    
## One Dimensional Arrays:
   ### Declaration of the array:
   Arrays can be declared like any other simple variables.
   
   __Syntax: _data_type_   array_name[size];__ 
   
   __Example: _int_ wt[10], _float_ height[20], _bool_ correct[20], where "wt", "height", "correct" are the array names.__ 
   
   So the syntax _float_ height[20] , means it is a floating value array and can store upto 20 such elements in it.
  
   __Points to keep in mind:__
   
   1) When an array is declared, the __amount of space that__ is need to hold all the elements is __allocated in the memory__.
   2) The __size of the array must be known during compilation time__.
   3) We __can't use any variables for specifying the size__ of the array. If it's a variable then __it's value must be known__.
  ### Accessing the elements:
  The elements in the array can be accessed by __specifying the array name and the index in brackets__. 
  
  __Index 0 is known as the lower bound__ of the array and the __last index is known as the upper bound__ of the array.
  
  So, for a integer array named "arr" of length 3, the elements would be arr[0], arr[1], arr[2]. 
  
  Over here, 0 is the lower bound and 2 is the upper bound.
  
  If we try to __access an index in the array which is outside of it's upper bound then it will give us an error__.
  
  Example:
  
  int arr=[3]; but we try to access arr[23], this is going to give us an error.
  
  ### Processing the array:
  To process an array, the most common way of doing it is to use a __for loop__.
  
  The loop variable is used in place of the index of the array. It __should start from 0__ , because we want to access the whole array and should __go on till the last index while incrementing by 1__.
  
   __Example:__
   1) For reading:
   
     for(int i=0;i<3;i++)
        scanf("%d", &arr[i]);
   2) For printing:
   
     for(int i=0;i<3;i++)
        printf("%d", arr[i]);
  ### Initialization of the array:
  After the initial declaration, __the elements of a local array have garbage(or default) values__ while the elements of __global and static arrays have value as 0__.
  
  __Syntax for initialization of array__: 
  
  ___data_type_   array_name[size] = { value1, value 2, value3, value4,...valueN};__
  
  Here, array_name is the variable name, size is the size and value1,value2,.. are initializers.
  
  _Note_: These values are seperated by commas and there's a semicolon after the ending bracket.
 
   While initializing an one-dimentisonal array, __it is optional to mention the size of it__.
   
   If not mentioned the __compiler assumes the size to be equal to the number of initializers__.
   
   _A few examples:_
   1) int arr[]={3,4,10}; over here the __size of the array "arr" is going to be 3__.

   2) int mad[10]={5,69,420,54}; over here we can see that the size of the array is specified to be 10 but there are only 5 initializers. In such cases, __the rest of the values are going to be initialized to 0 (garbage value)__. So mad[8] will be 0.
   
   3) int buzz[5]={4,12,356,69,123,432,23423}; this is not going to give us any error although over here the total number of initializers is more than the size of the array. In such cases, we are instead __going to get a warning__ and only those values of initializers will be stored __starting from 0 to last index of the size__. So, buzz[5] will be 123.
   
   __Now, let's do a quick check:__
   
   int arr[10]={0};
   
   What does it mean? 
   
   It means that the first element of the array is going to be equal to 0 and the rest of them are also going to be initialized with 0. 
   
   So __every value of this array is going to be 0__. arr[0]=0, arr[5]=0, arr[9]=0.
  
## Two Dimensional Arrays:

======================================================================

Article Title: Recursion Name: Abhishek Mishra Author Profile:https://github.com/mishra-abhii Date: 17-10-21

======================================================================

## What is Recursion? 
The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. 
Using recursive algorithm, certain problems can be solved quite easily. 
Examples of such problems are Towers of Hanoi (TOH), Inorder/Preorder/Postorder Tree Traversals, DFS of Graph, etc.

## What is base condition in recursion? 
In the recursive program, the solution to the base case is provided and the solution of the bigger problem is expressed in terms of smaller problems. 

-    int fact (int n) 
-    {
-      if (n < = 1)   // base case
         return 1;
       else    
         return n * fact(n-1);
-    }

In the above example, base case for n < = 1 is defined and larger value of number can be solved by converting to smaller one till base case is reached.

## How a particular problem is solved using recursion? 
The idea is to represent a problem in terms of one or more smaller problems, and add one or more base conditions that stop the recursion. 
For example, we compute factorial n if we know factorial of (n-1). The base case for factorial would be n = 0. We return 1 when n = 0. 

## How memory is allocated to different function calls in recursion? 
When any function is called from main(), the memory is allocated to it on the stack. 
A recursive function calls itself, the memory for a called function is allocated on top of memory allocated to calling function and different copy of local 
variables is created for each function call. When the base case is reached, the function returns its value to the function by whom it is called and 
memory is de-allocated and the process continues.

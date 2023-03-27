# Activities

## Task 1

> Refer to the following links while discussing the answer.

- What is the difference between `array` and `std::array`
  https://stackoverflow.com/questions/30263303/stdarray-vs-array-performance

> Using the std::array gives more functionality and makes the code easier for the compiler


- What is the difference between `std::array` and `std::vector`
  https://www.softwaretestinghelp.com/arrays-in-stl/

> Vector is dynamic, array static in size. Arrays are contiguous memory locations. Array container is a sequential homogenous container and is of a fixed size, which differenciates it from vector.


- What is the difference between `std::list` and `std::vector`
  https://www.softwaretestinghelp.com/lists-in-stl/

> List implements linked list in c++, this allows us to insert elements anywhere in the list without causing excess overhead.


## Task 2

- Run the Stack and Queue examples in the following link
  https://www.softwaretestinghelp.com/stacks-and-queues-in-stl/

> make sure you correct the syntax e.g `&lt;int&gt; becomes  <int>`
```cpp
#include <iostream>
#include <stack>
using namespace std;
void printStack(stack <int> stk)
{
   while (!stk.empty())
      {
         cout << '\t' << stk.top();
         stk.pop();
      }
   cout << '\n';
}
  
int main ()
{
   stack <int> oddstk;
   oddstk.push(1);
   oddstk.push(3);
   oddstk.push(5);
   oddstk.push(7);
   oddstk.push(9);
  
   cout << "The stack is :";
   printStack(oddstk);
  
   cout << "\nSize of stack:" << oddstk.size();
   cout << "\nTop of stack:" << oddstk.top();
   cout << "\noddstk.pop() : ";
   oddstk.pop();
   printStack(oddstk);
   cout <<"\nAnother pop(): ";
   oddstk.pop();
   printStack(oddstk);
   return 0;
}
```
```cpp
#include <iostream>
#include <queue>
using namespace std;
void printQueue(queue <int> myqueue)
{
   queue <int> secqueue = myqueue;
   while (!secqueue.empty())
   {
      cout <<'\t' << secqueue.front();
      secqueue.pop();
   }
   cout <<'\n';
}
int main()
   {
      queue <int> myqueue;
      myqueue.push(2);
      myqueue.push(4);
      myqueue.push(6);
      myqueue.push(8);
      cout << "The queue myqueue is : ";
      printQueue(myqueue);
      cout << "\nmyqueue.size() : " << myqueue.size();
      cout << "\nmyqueue.front() : " << myqueue.front();
      cout << "\nmyqueue.back() : " << myqueue.back();
      cout << "\nmyqueue.pop() : ";
      myqueue.pop();
      printQueue(myqueue);
      return 0;
   }
```
## Task 3

- Discuss the different types of iterators present in C++. You can refer to the following link
  https://www.geeksforgeeks.org/introduction-iterators-c/
> An iterator is an object (like a pointer) that points to an element inside the container. 
There are five major categories of iterators: input, output, forward, bidirectional, and random-access iterators. 

- What are the Benefits of Iterators
> convinience, code reusability, ability to dynamically add or remove elements from the container 

## Links

- https://cpp.sh/

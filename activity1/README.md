# Activities

---

> [Course Feedback](https://ojp.metropolia.fi/lomakkeet/1/lomake.html?code=VFQwMEZFMzktMzAwMQ==)

---

## Task 1

- What is the difference between function overloading and function templates. You can refer to the programs in the `./src/` folder as well as [Links 2 and 3](#links) below.

> In Function overloading the compiler knows which function to call (for example a different function for int and double). 
Function template automatically recognizes the type of the variable, so there's no need to use different functions for different variable types.

- Rewrite the following program using templates

```cpp
#include <iostream>
template <typename T> 

T add(T x, T y)
{
    return x + y;
}

/* int add(int x, int y)
{
    return x + y;
}

double add(double x, double y)
{
    return x + y;
} */

int main()
{
    std::cout << add(1, 2); // calls add
    std::cout << '\n';
    std::cout << add(1.2, 3.4); // calls add

    return 0;
}
```

## Task 2

Refer to the following link:
https://www.softwaretestinghelp.com/vectors-in-stl/

Discuss the difference between

- Size() and capacity()
> number of elements in a vector is size(), the capacity() is the amount of elements that the vector can hold. 

- begin() and cbegin()
> begin() iterates the vector from the beginning (first element). cbegin() means constant, that content can't be modified.

- end() and cend()
> end(): Returns an iterator pointing to the element that follows the last element in the vector.
cend(): Returns a constant iterator pointing to the element following the last element of the vector container.

## Links

1. https://cpp.sh/
2. https://www.learncpp.com/cpp-tutorial/function-templates/
3. https://www.learncpp.com/cpp-tutorial/function-overload-differentiation/
4. https://www.geeksforgeeks.org/design-and-analysis-of-algorithms/

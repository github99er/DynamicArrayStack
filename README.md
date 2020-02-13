# Implementing a Stack on a Dynamic Array
### Built With
* [Microsoft Visual Studio](https://visualstudio.microsoft.com/pl/) - IDE
* [C99](https://en.wikipedia.org/wiki/C99) - C Language Standard




# Introduction Stack Data Structure

A stack is a container abstraction that maintains values in order based on their time of insertion. When a value is removed from the stack it is the value that has been most recently added to the stack In a stack abstraction the only item we are allowed to access is the topmost item. Every time we add to the stack the previous item is in-accessible while the last one added is.
### Behaviors (methods) of a Stack:

| Behavior | README |
| ------ | ------ |
| Push | add new element to top of the stack |            
| Pop | remove element at top of the stack |   
| Top | return element at top of the stack |
| Empty| does the stack contain any elements |

### Visual of Stack Behaviors:
![](stack.png)        


### Real Life Stack Examples:
```sh
 1. Stack of plates     2. Stack of Glasses     3. Tennis ball packaging     4. Paper in a printer
```
# Introduction Static Array & Dynamic Array

### Dynamic Array Properties:
| Property | README |
| ------ | ------ |
| Size | The number of elements in the array at a given time  |
| Capacity | The number of elements the array can hold at a given time |

A static array is a container abstraction designed to hold a collection of elements that allows quick access to an element in the container. A static array has a fixed size which must be specified upon creation. A dynamic array is an abstraction of the static array, the difference being the capacity of the array is dynamically updated at runtime. Allocation at runtime allows for only necessary memory to be allocated.

### Why use a dynamic array?
- Using a dynamic array prevents overallocation of program memory
- If overallocated then program runs slower than necessary



### Dynamic Array Interface (important method(s) only):
```sh
void _dynArraySetCapacity (struct DynArr * da)
→ Given a pointer (da) to a dynamic array, double the dynamic array’s current capacity
```


### Stack Interface:



```sh
void dynArrayPush (struct DynArr * da, TYPE e) 
→ Given a value (e), add (e) to the top (rightmost) index of a dynamic array given the dynamic array's pointer (da)
→ Calls _dynArraySetCapacity when attempting to push to a dynamic array at full capacity

TYPE dynArrayTop (struct DynArr * da) 
→ Given a pointer (da) to a dynamic array, return the top (rightmost) element of the dynamic array

void dynArrayPop (struct DynArr * da) 
→ Given a pointer (da) to a dynamic array, remove the top (rightmost) index of the given dynamic array

int dynArrayIsEmpty (struct DynArr * da) 
→ Given a pointer (da) to a dynamic array, return 1 if the dynamic array contains zero elements and return 0 if not
```

### Compiling Methods Used

```sh
$ gcc -Wall -std=c99 -o filename filename.c 

Wall = show all warnings
std=c99 = ANSI standardized version of C99

```
### Contributor

* **Ryan Murphy** - [Github99er](https://github.com/Github99er)

#


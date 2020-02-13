# Implementing a Stack on a Dynamic Array

![](STACK.png)




# Introduction Stack:

A stack is a container abstraction that maintains values in order based on their time of insertion. When a value is removed from the stack it is the value that has been most recently added to the stack In a stack abstraction the only item we are allowed to access is the topmost item. Every time we add to the stack the previous item is in-accessible while the last one added is.
### Behaviors (methods) of a Stack:

| Behavior | README |
| ------ | ------ |
| Push | [plugins/dropbox/README.md][PlDb] |
| Pop | [plugins/github/README.md][PlGh] |
| Top | [plugins/dropbox/README.md][PlDb] |
| Empty| [plugins/github/README.md][PlGh] |

### Real Life Stack Examples:
```sh
 1. Stack of plates     2. Stack of Glasses     3. Tennis ball packaging     4. Paper in a printer
```
# Introduction Static Array & Dynamic Array

### Dynamic Array Properties:
| Property | README |
| ------ | ------ |
| Size | The number of elements in the array at a given time  |
| Capacity | The number of elements an array can hold at a given time |

A static array is a container abstraction designed to hold a collection of elements that allows quick access to an element in the container. A static array has a fixed size which must be specified upon creation. A dynamic array is an abstraction of the static array, the difference being the capacity of the array is dynamically updated at runtime. Allocation at runtime allows for only necessary memory to be allocated.

### Why use a dynamic array?
- Using a dynamic array prevents overallocation or underallocation of program memory. 
- If underallocated errors may be thrown, if overallocated then program runs slower than necessary



### Dynamic Array Interface (important method(s) only):
```sh
void _dynArraySetCapacity (struct DynArr * da)
→ When the capacity of a given array (da) has been reached, double the given array’s current capacity
```


### Stack Implementation Interface:



```sh
void dynArrayPush (struct DynArr * da, TYPE e) 
→ Adds a value (e) to the top (rightmost) index of a given dynamic array (da) and has no return value.

TYPE dynArrayTop (struct DynArr * da) 
→ Given dynamic array (da)  return value TYPE (TYPE will be of Int, Double, Float, Bool, Char);

void dynArrayPop (struct DynArr * da) 
→ Given dynamic array (da) remove the top (rightmost) index of the given dynamic array (da);

int dynArrayIsEmpty (struct DynArr * da) 
→ Given dynamic array (da) return 0 if the dynamic array contains zero elements and return 1 if not;
```

Compiling Methods used

```sh
$ npm install --production
$ NODE_ENV=production node app
```

#


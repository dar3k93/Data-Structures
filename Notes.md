- []()
- [Memory](#Memory)

# Complexity analysis

## Complexity analysis
A process of determinating of how efficient an algotithm is. Complexity analysis usually involves finding both the time complexity and the space complexity of an algorithm.

## Time Complexity 
A measure of how fast an algorithm runs. It is expressed using Big O notation

## Space Cmplexity
A measure of much much auxiliary memory an algorithm takes up. It's expressed using Big O notation

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Memory

## Bit
Short fot binary digit, a bit is a fundamnetal unit of information in Computer science that represents a state with one of two values: 0 or 1

## Byte
A group of eight bits. For example 01101000 is a byte. A single byte can represent up to 256 data values
Since a binary number is a number can be expressed with only two symbols: 0 and 1, a byte can effectively represent all of the numbers between 0 and 255, inclusive, in binary format. The following bytes represent the numbers 1,2,3 and 4 in bianry format:
1: 00000001
2: 00000010
3: 00000011
4: 00000100

## Fixed-With Integer
An Integer represented by a fixed amount of bites. For example a 32-bit integer is and integer represented by 32 bits (4-bytes) and 64-bit integer is an integer represented by 64 bits (8 bytes)


## Memory
Broadly speaking memory is the foundational layer of computing, where all data are stored
- Data stored in memory is stored in bytes and by extension bits
- Bytes in memory can point to other bytes in memory so as to store references to other data
- The amount of memory that a machine has is bounded, making it valeuable to limit how much memory an algorithm take up
- Accessing a byte or fixed number of bytes (like 4 or 8 bytes in this case 32 or 64 bit integers) is an elementary operation, which can be loosely treated as a single unit of operational work

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Big O notation

## Big O notation
The notation used to descibe the time complexity and space complexity of algorithms

Variables used in Big O notation denote the size of inputs to algorithms. For example, O(n) might be the time complexity of an algorithm that traverses through an array of length n; simiraly, O(n+m) might be the time complexity of na algorithm that traverses through an array of length n and through a string length m

Examples of common complexties and their big O:
- Constatnt O(1)
- Logarithm O(log(n))
- Lineral O(n)
- Log-lineral O(log(n))
- Quadratic O(n2)
- Cubic O(n3)
- Exponential O(2to n)
- Factorial O(n!)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Logarithms

## Logarithm

A mathematical concept that widely used in Computer Science and thats defined by the following equation:

![image](https://user-images.githubusercontent.com/49185097/212162177-9e655003-6500-4ec8-b824-fba6d319810d.png)

In the context of coding interviews the logarithm is used to describe the complexity analysis of algorithm and its useage always implies a logarithm of base 2. In other words. the logarithm used in the context of coding interviews is defined by the following equation:

![image](https://user-images.githubusercontent.com/49185097/212162242-2ef39886-416c-4193-b73c-85488548d515.png)

In plain English, if an algorithm has a logarithmc time complexity (O(log(n)), where n is the size of the input), then whenever the algorithm's input doubles in size (i.e., whenever n doubles), the number of operations needed to complete the algorithm only increase by one unit. Conversely, an algorithm with linerar time complexity would see its number of operations double if its input size doubled.

As an example, a linear-time complexity algorithm with an input size 1,000 might take roughly 1,000 iperations to complete wheres a logarithmic-time complexity algorithm with the same input would take roughly 10 operations to complete, since 210 ~= 1,000.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Arrays

## Array
A linear collection of data values that are accessible at numbered indices, starting at index 0

The following are an array's standard operations and their corresponding time complexities:
- Accessing a value at a gicen index: O(1)
- updating a value at given index: O(1)
- Inserting a value at the beginning: O(n)
- Inserting a value in the middle: O(n)
- Inserting a value at the end:
	- amortized O(1) when dealing with a dynamic array
	- O(n) when dealing with a static array
- Removing a value at the beginning: O(n)
- Removing a value in the middle: O(n)
- Removing a value at the end: O(1)
- Copying the array: O(n)

A static array is an implementation of an array that allocates a fixed amount of money of memory to be used for storing the array's values. Appending values the array therefore involves coping the entire array and allocating new memory fo it, accounting for the extra space needed for the newly appended value. This is a linear-time operation.

A dynamic array is an array that peemptiveky allocates double the amount of memory needed to store the arrayls values. Appending values to the array is a constant-time operation until the allocated memory is filled up, at which point the array is copied and double the momory is once again allocated fo it. This implementation leads to an amortized constat-time insertion-at-end operation

A lot of popular programming languages like JavaScript and Python implement arrays as dynamic arrays.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Strings

## Strings
One of the fundamental data types in Computer Science are stored in memory as arrays of integers, where each character in a given string is mapped
to an integer via some character standard like ASCII.

String behave much like normal arraysm with the main distinctionbeing that, in most programming languages (c++ is a noteable exception), string are immutable, meaning that they can not be edited after creation. This also means that simple operations like appanding a character to a string are more expensive than they might appear.

The canonical example of an operation that is deceprively expensive due to string immutabillity is the following:
```
string = "this is a string"
newString = ""

for character in string:
	newString += character
```

The operation above has a time complexity of O(n to 2) where n is the length of string, because each addition of a character to newString creates an entirely new string and is itself an O(n) operation. Therefore , n O(n) operations are performed , leading to an O(n to 2) time-complexity operational overall.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Graphs

## Graphs
A collection of nodes or values called vertices that might be related; relations between vertices are called edges.

Many things in life can be represented by graphs; for example a social network can be represented by a graph whose vertices are users and whose edges are friendship between the users. Similarly, a city map can be represented by a graph whose vertices are locations in the city whose edges are roads between the locations.

## Grap Cycle

## Acyclic Graph
A graph that has no cycles

## Cyclic Graph
A graph that has at least one cycle

## Directed Graph

## Undirected Graph

## Connected Graph






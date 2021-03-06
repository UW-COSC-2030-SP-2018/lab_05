Frederick Wittman

Dr. Hill

COSC 2030-01

25 March 2019

### 1.  To comment C++ code:

Inserting "//" will identify everything after this symbol as a comment on a single line.  To add a block comment that can span multiple lines, insert the desired comment between the asterisks of the "/* */" symbol.
    
### 2.  To comment Python code:

The "#" symbol is used to comment out a single line.  To identify a block of code as a comment, insert the code between three
double quotation marks, literally: """comment""".
    
### 3.  What kind of file has extension ".md"?

Markdown files have extension ".md".  Markdown languages control the styling of webpages and other computer interfaces using
plain text.  The primary example of a markdown language is HTML.
    

### 4.  How to strip whitespace from the end of a string in C++:
    One way to strip the whitespace from the end of a string in C++ is to use the algorithm provided by the pixel compressor file:
    
#include <string>
    
string whitespace(" \t\f\v\n\r");  // Define whitespace characters
    
sampleString.substr(0, sampleString.find_last_not_of(whitespace));

This returns a substring beginning at the zeroth element of sampleString and ending at the last character in sampleString that is not the parameter, which in this case is whitespace, of the the find_last_not_of function.  Note that this function will not strip whitespace inside the string, but only whitespace
that trails the last character.

### 5.  How to create an object of type T and its pointer:

Generically, without formatting and in connection to a function or class you need the following:

template <class T>
T object;
T * objectPtr = &object;
    
### 6.  List the Python modules that you have imported in your Python experience, and what they contain. And answer this question: What is the class of the ops variable? (Review Ch. 5 of the Tutorial.) And what are the other general-purpose built-in container data structures in Python?
    
I have imported the math and operations modules.  The ops variable is a set.  In addition to sets, Python supports tuples,
sequences, and lists. Additionally, lists can be used as the substrate for stacks and queues.

### 7.  How to declare a record structure in C++:

Records are linear, direct access data structures with heterogenous components.  In C++, they are declared as structs:

struct {

type1 field1; 

type2 field2;

...}

### 8.  How to declare a binary tree in C++ and Python:

##### C++
```
struct Node{
	int value;
	struct Node * rightNode = NULL;
	struct Node * leftNode = NULL;
};

Node * root = new Node;
root->value = 5;
```
##### Python
```
class Node:

    def __init__(self, value):

    	self.left = None
    	self.right = None
    	self.value = value

root = Node(5)
```

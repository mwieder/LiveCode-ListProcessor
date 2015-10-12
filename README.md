# LiveCode-ListProcessor

Simple list processing - first, last, next, prior, head, tail, ahead, behind, peek, poke, remove, append, insert, etc..

The current implementation of ListProcessor uses LiveCode arrays to store a list and its index. The design and code have not been optimised in anyway. My first objective is to get basic list processing working and then to improve on it. 

## Currently implemented functions

### LP.makeList
This function creates a list. A variable in which to "put" the created list.
```
  arguments
    pStringList     The items to put in the list
    pDelimiter      The separator used in the string between items in the list
  returns           The list or empty
```

### LP.head
Sets the index to the first item and returns the first item
```
  argument
    pList         The list
  returns         The first item in the list or empty
```

### LP.head?
Returns true if the index is set to the first item in the list
```
  argument
    pList         The list
  returns         True or false
```

### LP.length?
Returns the number of items in the list based on the current index
```
  argument
    pList         The list
  returns         The number of items in the list from the current index
```
### LP.index?
Returns the value of the current index
```
  argument
    pList         The list
  returns         The value of the current index
```
### LP.next
Moves to the next item in the list and returns that item or empty
```
  argument
    pList         The list
  returns         The now first item or empty
```
### LP.peek
Returns the nth item based on the current index
```
  arguments
    pList         The list
    pPos          The position of the element requested
  returns         The item or empty
```

### LP.peek
Returns the nth item based on the current index
```
  arguments
    pList         The list
    pPos          The position of the element requested
  returns         The item or empty
```
  
### LP.prior
Moves to the prior item in the list and returns that item or empty
```
  argument
    pList         The list
  returns         The now first item or empty
```

### LP.tail
Sets the index to the last item and returns the last item
```
  argument
    pList         The list
  returns         The last item in the list or empty
```
### LP.tail?
Returns true if the index is set to the last item in the list
```
argument
  pList         The list
  returns       True or false
```

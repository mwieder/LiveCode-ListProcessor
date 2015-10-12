# LiveCode-ListProcessor

Simple list processing - first, last, next, prior, head, tail, ahead, behind, peek, poke, remove, append, insert, etc..

The current implementation of ListProcessor uses LiveCode arrays to store a list and its index. The design and code have not been optimised in anyway. My first objective is to get basic list processing working and then to improve on it. 

## Currently implemented functions

### LP.makeList
This function creates a list. A variable in which to "put" the created list.

  pStringList     The items to put in the list
  pDelimiter      The separator used in the string between items in the list
  returns         true if successful

### LP.length? - returns the number of items in the list based on the current index
  pList         The list
  returns       The number of items in the list from the current index
  
### LP.index? - returns the value of the current index
  pList         The list
  returns       The value of the current index
  
### LP.next - moves to the next item in the list and returns that item or empty
  pList         The list
  returns       The now first item or empty
  
### LP.peek - returns the nth item based on the current index
  pList         The list
  pPos          The position of the element requested
  returns       The item or empty
  
### LP.prior - moves to the prior item in the list and returns that item or empty
  pList         The list
  returns       The now first item or empty
  
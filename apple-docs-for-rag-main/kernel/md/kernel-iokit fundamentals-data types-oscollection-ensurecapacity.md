

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollection
-  ensureCapacity 

# ensureCapacity

Ensures the collection has enough space to store the requested number of objects.

``` source
virtual unsigned int ensureCapacity(
 unsigned intnewCapacity) = 0; 
```

## Parameters 

`newCapacity`  

The total number of objects the collection should be able to store.

## Return Value

The new capacity of the collection, which may be different from the number requested (if smaller, reallocation of storage failed).

## Overview

Subclasses implement this pure virtual member function to adjust their storage so that they can hold at least `newCapacity` objects. Libkern collections generally allocate storage in multiples of their capacity increment.

Subclass methods that add objects to the collection should call this function before adding any object, and should check the return value for success.

Collection subclasses may reduce their storage when the number of contained objects falls below some threshold, but no Libkern collections currently do.

## See Also

### Miscellaneous

copyCollection

Creates a deep copy of a collection.

flushCollection

Empties the collection, releasing any objects retained.

getCapacity

Returns the number of objects the collection can store without reallocating.

getCapacityIncrement

Returns the storage increment of the collection.

getCount

Returns the number of objects in the collection.

getNextObjectForIterator

Returns the next member of a collection.

haveUpdated

Tracks updates to the collection.

init

Initializes the OSCollection object.

initIterator

Initializes the iteration context for a collection subclass.

iteratorSize

Returns the size in bytes of a subclass's iteration context.

setCapacityIncrement

Sets the storage increment of the collection.


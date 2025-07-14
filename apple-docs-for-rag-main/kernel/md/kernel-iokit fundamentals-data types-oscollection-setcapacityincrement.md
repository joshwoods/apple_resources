

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollection
-  setCapacityIncrement 

# setCapacityIncrement

Sets the storage increment of the collection.

``` source
virtual unsigned int setCapacityIncrement(
 unsigned increment) = 0; 
```

## Return Value

The new storage increment of the collection, which may be different from the number requested.

## Overview

Subclasses must implement this pure virtual member function. Most collection subclasses allocate their storage in multiples of the capacity increment.

Collection subclasses should gracefully handle an `increment` of zero by applying (and returning) a positive minimum capacity.

Setting the capacity increment does not trigger an immediate adjustment of a collection's storage.

See ensureCapacity for how the capacity increment is used.

## See Also

### Miscellaneous

copyCollection

Creates a deep copy of a collection.

ensureCapacity

Ensures the collection has enough space to store the requested number of objects.

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


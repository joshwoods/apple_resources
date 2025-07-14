

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollection
-  getCount 

# getCount

Returns the number of objects in the collection.

``` source
virtual unsigned int getCount() const = 0; 
```

## Return Value

The number of objects in the collection.

## Overview

Subclasses must implement this pure virtual member function.

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


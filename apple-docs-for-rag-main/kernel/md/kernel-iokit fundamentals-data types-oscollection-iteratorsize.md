

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollection
-  iteratorSize 

# iteratorSize

Returns the size in bytes of a subclass's iteration context.

``` source
virtual unsigned int iteratorSize() const = 0; 
```

## Return Value

The size in bytes of the iteration context needed by the subclass of OSCollection.

## Overview

This pure virtual member function, which subclasses must implement, is called by an OSCollectionIterator object so that it can allocate the storage needed for the iteration context. An iteration context contains the data necessary to iterate through the collection.

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

setCapacityIncrement

Sets the storage increment of the collection.




- Kernel
- IOKit Fundamentals
- Data Types
- OSCollection
-  initIterator 

# initIterator

Initializes the iteration context for a collection subclass.

``` source
virtual bool initIterator(
 void *iterationContext) const = 0; 
```

## Parameters 

`iterationContext`  

The iteration context to initialize.

## Return Value

`true` if initialization was successful, `false` otherwise.

## Overview

This pure virtual member function, which subclasses must implement, is called by an OSCollectionIterator object to initialize an iteration context for a collection. The collection object should interpret `iterationContext` appropriately and initialize its contents to begin an iteration.

This function can be called repeatedly for a given context, whenever the iterator is reset via the OSCollectionIterator::reset function.

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

iteratorSize

Returns the size in bytes of a subclass's iteration context.

setCapacityIncrement

Sets the storage increment of the collection.


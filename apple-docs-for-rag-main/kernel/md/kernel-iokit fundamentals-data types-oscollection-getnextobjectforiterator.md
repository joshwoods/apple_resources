

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollection
-  getNextObjectForIterator 

# getNextObjectForIterator

Returns the next member of a collection.

``` source
virtual bool getNextObjectForIterator( 
 void *iterationContext, 
 OSObject **nextObject) const = 0; 
```

## Parameters 

`iterationContext`  

The iteration context.

`nextObject`  

The object returned by reference to the caller.

## Return Value

`true` if an object was found, `false` otherwise.

## Overview

This pure virtual member function, which subclasses must implement, is called by an OSCollectionIterator to get the next object for a given iteration context. The collection object should interpret `iterationContext` appropriately, advance the context from its current object to the next object (if it exists), return that object by reference in `nextObject`, and return `true` for the function call. If there is no next object, the collection object must return `false`.

For associative collections, the object returned should be the key used to access its associated value, and not the value itself.

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


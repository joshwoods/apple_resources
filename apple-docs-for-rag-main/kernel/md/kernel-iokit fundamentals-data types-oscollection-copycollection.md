

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollection
-  copyCollection 

# copyCollection

Creates a deep copy of a collection.

``` source
virtual OSCollection *copyCollection(
 OSDictionary *cycleDict = 0); 
```

## Parameters 

`cycleDict`  

A dictionary of all of the collections that have been copied so far, to start the copy at the top level pass `NULL` for `cycleDict`.

## Return Value

The newly copied collecton, `NULL` on failure.

## Overview

This function copies the collection and all of the contained collections recursively. Objects that are not derived from OSCollection are retained rather than copied.

Subclasses of OSCollection must override this function to properly support deep copies.

## See Also

### Miscellaneous

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

setCapacityIncrement

Sets the storage increment of the collection.


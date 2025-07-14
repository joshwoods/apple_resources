

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollection
-  haveUpdated 

# haveUpdated

Tracks updates to the collection.

``` source
void haveUpdated(); 
```

## Overview

Subclasses call this function *before* making any change to their contents (not after, as the name implies). Update tracking is used for collection iterators, and to enforce certain protections in the IORegistry.

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

init

Initializes the OSCollection object.

initIterator

Initializes the iteration context for a collection subclass.

iteratorSize

Returns the size in bytes of a subclass's iteration context.

setCapacityIncrement

Sets the storage increment of the collection.




- Kernel
- IOKit Fundamentals
- Data Types
- OSCollectionIterator
-  getNextObject 

# getNextObject

Advances to and returns the next object in the iteration.

``` source
virtual OSObject * getNextObject(); 
```

## Return Value

The next object in the iteration context, `NULL` if there is no next object or if the iterator is no longer valid.

## Overview

This function first calls isValid and returns `NULL` if that function returns `false`.

Subclasses must implement this pure virtual function to check for validity with isValid, and then to advance the iteration context to the next object (if any) and return that next object, or `NULL` if there is none.

## See Also

### Miscellaneous

free

Releases or deallocates any resources used by the OSCollectionIterator object.

initWithCollection

Initializes an OSCollectionIterator for the provided collection object.

isValid

Checks that the collection hasn't been modified during iteration.

reset

Resets the iterator to the beginning of the collection, as if it had just been created.

withCollection

Creates and initializes an OSCollectionIterator for the provided collection object.


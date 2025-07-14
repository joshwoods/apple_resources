

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollectionIterator
-  initWithCollection 

# initWithCollection

Initializes an OSCollectionIterator for the provided collection object.

``` source
virtual bool initWithCollection(
 const OSCollection *inColl); 
```

## Parameters 

`inColl`  

The OSCollection-derived collection object to be iteratated.

## Return Value

`true` if the initialization was successful, or `false` on failure.

## Overview

Not for general use. Use the static instance creation method withCollection instead.

## See Also

### Miscellaneous

free

Releases or deallocates any resources used by the OSCollectionIterator object.

getNextObject

Advances to and returns the next object in the iteration.

isValid

Checks that the collection hasn't been modified during iteration.

reset

Resets the iterator to the beginning of the collection, as if it had just been created.

withCollection

Creates and initializes an OSCollectionIterator for the provided collection object.


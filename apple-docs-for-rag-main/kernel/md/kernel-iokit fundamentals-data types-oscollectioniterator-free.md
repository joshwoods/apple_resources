

- Kernel
- IOKit Fundamentals
- Data Types
- OSCollectionIterator
-  free 

# free

Releases or deallocates any resources used by the OSCollectionIterator object.

``` source
virtual void free(); 
```

## Overview

This function should not be called directly; use release instead.

## See Also

### Miscellaneous

getNextObject

Advances to and returns the next object in the iteration.

initWithCollection

Initializes an OSCollectionIterator for the provided collection object.

isValid

Checks that the collection hasn't been modified during iteration.

reset

Resets the iterator to the beginning of the collection, as if it had just been created.

withCollection

Creates and initializes an OSCollectionIterator for the provided collection object.


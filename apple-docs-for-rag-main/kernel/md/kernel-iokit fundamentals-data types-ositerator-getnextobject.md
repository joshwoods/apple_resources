

- Kernel
- IOKit Fundamentals
- Data Types
- OSIterator
-  getNextObject 

# getNextObject

Advances to and returns the next object in the iteration.

``` source
virtual OSObject *getNextObject() = 0; 
```

## Return Value

The next object in the iteration context, `NULL` if there is no next object or if the iterator is no longer valid.

## Overview

The returned object will be released if removed from the collection; if you plan to store the reference, you should call retain on that object.

Subclasses must implement this pure virtual function to check for validity with isValid, and then to advance the iteration context to the next object (if any) and return that next object, or `NULL` if there is none.

## See Also

### Miscellaneous

isValid

Check that the collection hasn't been modified during iteration.

reset

Resets the iterator to the beginning of the collection, as if it had just been created.


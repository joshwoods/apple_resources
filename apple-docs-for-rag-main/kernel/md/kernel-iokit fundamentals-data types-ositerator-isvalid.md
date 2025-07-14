

- Kernel
- IOKit Fundamentals
- Data Types
- OSIterator
-  isValid 

# isValid

Check that the collection hasn't been modified during iteration.

``` source
virtual bool isValid() = 0; 
```

## Return Value

`true` if the iterator is valid for continued use, `false` otherwise (typically because the collection being iterated has been modified).

## Overview

Subclasses must implement this pure virtual member function.

## See Also

### Miscellaneous

getNextObject

Advances to and returns the next object in the iteration.

reset

Resets the iterator to the beginning of the collection, as if it had just been created.


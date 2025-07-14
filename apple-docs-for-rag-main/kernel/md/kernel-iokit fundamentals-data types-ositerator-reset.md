

- Kernel
- IOKit Fundamentals
- Data Types
- OSIterator
-  reset 

# reset

Resets the iterator to the beginning of the collection, as if it had just been created.

``` source
virtual void reset() = 0; 
```

## Overview

Subclasses must implement this pure virtual member function.

## See Also

### Miscellaneous

getNextObject

Advances to and returns the next object in the iteration.

isValid

Check that the collection hasn't been modified during iteration.


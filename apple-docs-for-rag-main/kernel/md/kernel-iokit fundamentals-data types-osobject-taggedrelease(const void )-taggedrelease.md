

- Kernel
- IOKit Fundamentals
- Data Types
- OSObject
-  taggedRelease(const void \*) 

# taggedRelease(const void \*)

Releases a tagged reference to an object, freeing it immediately if the reference count drops to zero.

``` source
virtual void taggedRelease(
 const void *tag = 0) const; 
```

## Parameters 

`tag`  

Used for tracking collection references.

## Overview

Kernel extensions should not use this function. It is for use by OSCollection and subclasses to track inclusion in collections.

## See Also

### Miscellaneous

free

Deallocates/releases resources held by the object.

getRetainCount

Returns the reference count of the object.

init

Initializes a newly-allocated object.

operator delete

Frees the memory of the object itself.

operator new

Allocates memory for an instance of the class.

release()

Releases a reference to the object, freeing it immediately if the reference count drops to zero.

release(int)

Releases a reference to an object, freeing it immediately if the reference count drops below the specified threshold.

retain

Retains a reference to the object.

serialize

Overridden by subclasses to archive the receiver into the provided OSSerialize object.

taggedRelease(const void *, const int)

Releases a tagged reference to an object, freeing it immediately if the reference count drops below the specified threshold.

taggedRetain

Retains a reference to the object with an optional tag used for reference-tracking.


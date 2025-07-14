

- Kernel
- IOKit Fundamentals
- Data Types
- OSObject
-  release() 

# release()

Releases a reference to the object, freeing it immediately if the reference count drops to zero.

``` source
virtual void release() const; 
```

## Overview

This function decrements the reference count of the receiver by 1. If the reference count drops to zero, the object is immediately freed using free.

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

release(int)

Releases a reference to an object, freeing it immediately if the reference count drops below the specified threshold.

retain

Retains a reference to the object.

serialize

Overridden by subclasses to archive the receiver into the provided OSSerialize object.

taggedRelease(const void *)

Releases a tagged reference to an object, freeing it immediately if the reference count drops to zero.

taggedRelease(const void *, const int)

Releases a tagged reference to an object, freeing it immediately if the reference count drops below the specified threshold.

taggedRetain

Retains a reference to the object with an optional tag used for reference-tracking.


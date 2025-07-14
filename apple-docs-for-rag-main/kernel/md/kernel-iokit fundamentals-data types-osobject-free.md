

- Kernel
- IOKit Fundamentals
- Data Types
- OSObject
-  free 

# free

Deallocates/releases resources held by the object.

``` source
virtual void free(); 
```

## Overview

Classes derived from OSObject should override this function to deallocate or release all dynamic resources held by the instance, then call the superclass's implementation.

**Caution:**

1.  You can not assume that you have completed initialization before `free` is called, so be very careful in your implementation.

2.  OSObject's implementation performs the C++ `delete` of the instance, so be sure that you call the superclass implementation *last* in your implementation.

3.  `free` must not fail; all resources must be deallocated or released on completion.

## See Also

### Miscellaneous

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

taggedRelease(const void *)

Releases a tagged reference to an object, freeing it immediately if the reference count drops to zero.

taggedRelease(const void *, const int)

Releases a tagged reference to an object, freeing it immediately if the reference count drops below the specified threshold.

taggedRetain

Retains a reference to the object with an optional tag used for reference-tracking.


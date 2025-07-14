

- Kernel
- IOKit Fundamentals
- Data Types
- OSObject
-  operator delete 

# operator delete

Frees the memory of the object itself.

``` source
static void operator delete(
 void *mem,
 size_tsize); 
```

## Parameters 

`mem`  

A pointer to the object's memory.

`size`  

The size of the object's block of memory.

## Overview

Never use `delete` on objects derived from OSObject; use release instead.

## See Also

### Miscellaneous

free

Deallocates/releases resources held by the object.

getRetainCount

Returns the reference count of the object.

init

Initializes a newly-allocated object.

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


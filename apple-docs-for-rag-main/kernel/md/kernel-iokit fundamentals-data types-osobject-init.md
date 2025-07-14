

- Kernel
- IOKit Fundamentals
- Data Types
- OSObject
-  init 

# init

Initializes a newly-allocated object.

``` source
virtual bool init(); 
```

## Return Value

`true` on success, `false` on failure.

## Overview

Classes derived from OSObject must override the primary init method of their parent. In general most implementations call super`::init()` before doing local initialisation. If the superclass call fails then return `false` immediately. If the subclass encounters a failure then it should return `false`.

## See Also

### Miscellaneous

free

Deallocates/releases resources held by the object.

getRetainCount

Returns the reference count of the object.

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




- Kernel
- IOKit Fundamentals
- Data Types
- OSObject
-  serialize 

# serialize

Overridden by subclasses to archive the receiver into the provided OSSerialize object.

``` source
virtual bool serialize(
 OSSerialize *serializer) const; 
```

## Parameters 

`serializer`  

The OSSerialize object.

## Return Value

`true` if serialization succeeds, `false` if not.

## Overview

OSObject's implementation writes a string indicating that the class of the object receiving the function call is not serializable. Subclasses that can meaningfully encode themselves in I/O Kit-style property list XML can override this function to do so. See OSSerialize for more information.

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

taggedRelease(const void *)

Releases a tagged reference to an object, freeing it immediately if the reference count drops to zero.

taggedRelease(const void *, const int)

Releases a tagged reference to an object, freeing it immediately if the reference count drops below the specified threshold.

taggedRetain

Retains a reference to the object with an optional tag used for reference-tracking.


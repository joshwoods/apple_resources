

- Kernel
- IOKit Fundamentals
- Data Types
- OSBoolean
-  free 

# free

Overridden to prevent deallocation of the shared global instances.

``` source
virtual void free(); 
```

## Overview

This function should never be called.

## See Also

### Miscellaneous

getValue

Returns the C++ `bool` value for the OSBoolean object.

isEqualTo(const OSBoolean *)

Tests the equality of two OSBoolean objects.

isEqualTo(const OSMetaClassBase *)

Tests the equality an OSBoolean to an arbitrary object.

isFalse

Checks whether the OSBoolean object represents a `false`` bool` value.

isTrue

Checks whether the OSBoolean object represents a `true`` bool` value.

serialize

Archives the receiver into the provided OSSerialize object.

taggedRelease

Overrides the reference counting mechanism for the shared global instances.

taggedRetain

Overrides the reference counting mechanism for the shared global instances.

withBoolean

Returns one of the global instances of OSBoolean.


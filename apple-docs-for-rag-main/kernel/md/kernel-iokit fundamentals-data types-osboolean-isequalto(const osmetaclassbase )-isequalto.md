

- Kernel
- IOKit Fundamentals
- Data Types
- OSBoolean
-  isEqualTo(const OSMetaClassBase \*) 

# isEqualTo(const OSMetaClassBase \*)

Tests the equality an OSBoolean to an arbitrary object.

``` source
virtual bool isEqualTo(
 const OSMetaClassBase *anObject) const; 
```

## Parameters 

`anObject`  

An object to be compared against the receiver.

## Return Value

`true` if the objects are equal, `false` if not.

## Overview

An OSBoolean is considered equal to another object if that object is derived from OSBoolean and represents the same C++ `bool` value.

## See Also

### Miscellaneous

free

Overridden to prevent deallocation of the shared global instances.

getValue

Returns the C++ `bool` value for the OSBoolean object.

isEqualTo(const OSBoolean *)

Tests the equality of two OSBoolean objects.

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


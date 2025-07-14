

- Kernel
- IOKit Fundamentals
- Data Types
- OSBoolean
-  isEqualTo(const OSBoolean \*) 

# isEqualTo(const OSBoolean \*)

Tests the equality of two OSBoolean objects.

``` source
virtual bool isEqualTo(
 const OSBoolean *aBoolean) const; 
```

## Parameters 

`aBoolean`  

The OSBoolean to be compared against the receiver.

## Return Value

`true` if the OSBoolean objects are equal, `false` if not.

## Overview

Two OSBoolean objects are considered equal if they are the same exact object (pointer equality).

## See Also

### Miscellaneous

free

Overridden to prevent deallocation of the shared global instances.

getValue

Returns the C++ `bool` value for the OSBoolean object.

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


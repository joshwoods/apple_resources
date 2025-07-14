

- Kernel
- IOKit Fundamentals
- Data Types
- OSBoolean
-  withBoolean 

# withBoolean

Returns one of the global instances of OSBoolean.

``` source
static OSBoolean * withBoolean(
 boolvalue); 
```

## Parameters 

`value`  

A boolean value.

## Return Value

The global instance of OSBoolean with the boolean `value`.

## Overview

This function actually returns either kOSBooleanTrue or kOSBooleanFalse, so that you can always use pointer comparison with OSBoolean objects.

## See Also

### Miscellaneous

free

Overridden to prevent deallocation of the shared global instances.

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


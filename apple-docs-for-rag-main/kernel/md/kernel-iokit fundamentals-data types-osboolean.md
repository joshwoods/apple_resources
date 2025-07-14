

- Kernel
- IOKit Fundamentals
- Data Types
-  OSBoolean 

Class

# OSBoolean

OSBoolean wraps a boolean value in a C++ object for use in Libkern collections.

macOS 10.0+

``` source
class OSBoolean : OSObject
```

## Overview

OSBoolean represents a boolean `true`/`false` value as a Libkern C++ object. There are only two instances of OSBoolean, kOSBooleanTrue and kOSBooleanFalse. These are shared globally and returned by the instance-creation function withBoolean. Thus, you can use pointer comparison to test whether two OSBoolean objects are equal.

## Topics

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

withBoolean

Returns one of the global instances of OSBoolean.

### Instance Methods

- free

- getMetaClass

- getValue

- isEqualTo

- isEqualTo

- isFalse

- isTrue

- serialize

- taggedRelease

- taggedRetain

### Type Methods

+ initialize

+ withBoolean

## Relationships

### Inherits From

- OSObject

## See Also

### Simple Types

OSString

OSString wraps a C string in a C++ object for use in Libkern collections.

OSNumber

OSNumber wraps an integer value in a C++ object for use in Libkern collections.

OSData

OSData wraps an array of bytes in a C++ object for use in Libkern collections.


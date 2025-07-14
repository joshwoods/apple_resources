

- Kernel
- IOKit Fundamentals
- Data Types
- OSString
-  isEqualTo(const OSMetaClassBase \*) 

# isEqualTo(const OSMetaClassBase \*)

Tests the equality of an OSString object to an arbitrary object.

``` source
virtual bool isEqualTo(
 const OSMetaClassBase *anObject) const; 
```

## Parameters 

`anObject`  

The object to be compared against the receiver.

## Return Value

Returns `true` if the two objects are equivalent, `false` otherwise.

## Overview

An OSString is considered equal to another object if that object is derived from OSString and contains the equivalent bytes of the same length.

## See Also

### Miscellaneous

free

Deallocates or releases any resources used by the OSString instance.

getChar

Returns the character at a given index in the string object.

getCStringNoCopy

Returns a pointer to the internal C string buffer.

getLength

Returns the number of characters in the OSString object.

initWithCString

Initializes an OSString from a C string.

initWithCStringNoCopy

Initializes an immutable OSString to share the provided C string buffer.

initWithString

Initializes an OSString from another OSString.

isEqualTo(const char *)

Tests the equality of an OSString object with a C string.

isEqualTo(const OSData *)

Tests the equality of an OSData object and the OSString instance.

isEqualTo(const OSString *)

Tests the equality of two OSString objects.

serialize

Archives the receiver into the provided OSSerialize object.

setChar

Replaces a character at a given index in the string object.

withCString

Creates and initializes an OSString from a C string.

withCStringNoCopy

Creates and initializes an immutable OSString that shares the provided C string buffer.

withString

Creates and initializes an OSString from another OSString.


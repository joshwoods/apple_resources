

- Kernel
- IOKit Fundamentals
- Data Types
- OSString
-  initWithCString 

# initWithCString

Initializes an OSString from a C string.

``` source
virtual bool initWithCString(
 const char *cString); 
```

## Parameters 

`cString`  

The C string to copy into the new OSString.

## Return Value

`true` on success, `false` on failure.

## Overview

Not for general use. Use the static instance creation method withCString instead.

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

initWithCStringNoCopy

Initializes an immutable OSString to share the provided C string buffer.

initWithString

Initializes an OSString from another OSString.

isEqualTo(const char *)

Tests the equality of an OSString object with a C string.

isEqualTo(const OSData *)

Tests the equality of an OSData object and the OSString instance.

isEqualTo(const OSMetaClassBase *)

Tests the equality of an OSString object to an arbitrary object.

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




- Kernel
- IOKit Fundamentals
- Data Types
- OSString
-  initWithCStringNoCopy 

# initWithCStringNoCopy

Initializes an immutable OSString to share the provided C string buffer.

``` source
virtual bool initWithCStringNoCopy(
 const char *cString); 
```

## Parameters 

`cString`  

The C string to reference.

## Return Value

`true` on success, `false` on failure.

## Overview

Not for general use. Use the static instance creation method withCStringNoCopy instead.

An OSString object initialized with this function does not claim ownership of the C string, but shares it with the caller. When the caller determines that the OSString object has actually been freed, it can safely dispose of the data buffer. Conversely, if it frees the shared data buffer, it must not attempt to use the OSString object and should release it.

An OSString object created with this function does not allow changing the string via setChar.

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


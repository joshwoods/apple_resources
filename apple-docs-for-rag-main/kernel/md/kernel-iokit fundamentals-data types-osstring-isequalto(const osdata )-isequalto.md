

- Kernel
- IOKit Fundamentals
- Data Types
- OSString
-  isEqualTo(const OSData \*) 

# isEqualTo(const OSData \*)

Tests the equality of an OSData object and the OSString instance.

``` source
virtual bool isEqualTo(
 const OSData *aDataObject) const; 
```

## Parameters 

`aDataObject`  

An OSData object.

## Return Value

`true` if the two objects are equivalent, `false` otherwise.

## Overview

This function compares the bytes of the OSData object against those of the OSString, accounting for the possibility that an OSData might explicitly include a nul character as part of its total length. Thus, for example, an OSData object containing either the bytes \ or \ will compare as equal to the OSString containing "usb".

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


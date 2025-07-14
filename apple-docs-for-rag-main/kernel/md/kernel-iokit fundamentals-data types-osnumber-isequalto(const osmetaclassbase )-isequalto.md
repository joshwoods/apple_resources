

- Kernel
- IOKit Fundamentals
- Data Types
- OSNumber
-  isEqualTo(const OSMetaClassBase \*) 

# isEqualTo(const OSMetaClassBase \*)

Tests the equality an OSNumber to an arbitrary object.

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

An OSNumber is considered equal to another object if that object is derived from OSNumber and represents the same C integer value.

## See Also

### Miscellaneous

addValue

Adds a signed integer value to the internal integer value of the OSNumber object.

free

Deallocates or releases any resources used by the OSNumber instance.

init(const char *, unsigned int)

Initializes an instance of OSNumber with an unsigned integer value represented as a C string.

init(unsigned long long, unsigned int)

Initializes an instance of OSNumber with an integer value.

isEqualTo(const OSNumber *)

Tests the equality of two OSNumber objects.

numberOfBits

Returns the number of bits used to represent the OSNumber object's integer value.

numberOfBytes

Returns the number of bytes used to represent the OSNumber object's integer value.

serialize

Archives the receiver into the provided OSSerialize object.

setValue

Replaces the current internal integer value of the OSNumber object by the value given.

unsigned16BitValue

Returns the OSNumber object's integer value cast as an unsigned 16-bit integer.

unsigned32BitValue

Returns the OSNumber object's integer value cast as an unsigned 32-bit integer.

unsigned64BitValue

Returns the OSNumber object's integer value cast as an unsigned 64-bit integer.

unsigned8BitValue

Returns the OSNumber object's integer value cast as an unsigned 8-bit integer.

withNumber(const char *, unsigned int)

Creates and initializes an instance of OSNumber with an unsigned integer value represented as a C string.

withNumber(unsigned long long, unsigned int)

Creates and initializes an instance of OSNumber with an integer value.




- Kernel
- IOKit Fundamentals
- Data Types
- OSNumber
-  numberOfBits 

# numberOfBits

Returns the number of bits used to represent the OSNumber object's integer value.

``` source
virtual unsigned int numberOfBits() const; 
```

## Return Value

The number of bits used to represent the OSNumber object's integer value.

## Overview

The number of bits is used to limit the stored value of the OSNumber. Any change to its value is performed as an `unsigned long long` and then truncated to the number of bits.

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

isEqualTo(const OSMetaClassBase *)

Tests the equality an OSNumber to an arbitrary object.

isEqualTo(const OSNumber *)

Tests the equality of two OSNumber objects.

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


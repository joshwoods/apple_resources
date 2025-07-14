

- Kernel
- IOKit Fundamentals
- Data Types
- OSNumber
-  withNumber(const char \*, unsigned int) 

# withNumber(const char \*, unsigned int)

Creates and initializes an instance of OSNumber with an unsigned integer value represented as a C string.

``` source
static OSNumber * withNumber( 
 const char *valueString, 
 unsigned intnumberOfBits); 
```

## Parameters 

`valueString`  

A C string representing a numeric value for the OSNumber to store.

`numberOfBits`  

The number of bits to limit storage to.

## Return Value

An instance of OSNumber with a reference count of 1; `NULL` on failure.

## Overview

This function does not work in I/O Kit versions prior to 8.0 (OS X 10.4). In I/O Kit version 8.0 and later, it works but is limited to parsing unsigned 32 bit quantities. The format of the C string may be decimal, hexadecimal ("0x" prefix), binary ("0b" prefix), or octal ("0" prefix).

The parsed value is masked to the provided `numberOfBits` when the OSNumber object is initialized.

You can change the value of an OSNumber later using setValue and addValue, but you can't change the bit size.

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

withNumber(unsigned long long, unsigned int)

Creates and initializes an instance of OSNumber with an integer value.


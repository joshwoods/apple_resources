

- Kernel
- IOKit Fundamentals
- Data Types
-  OSNumber 

Class

# OSNumber

OSNumber wraps an integer value in a C++ object for use in Libkern collections.

macOS 10.0+

``` source
class OSNumber : OSObject
```

## Overview

OSNumber represents an integer of 8, 16, 32, or 64 bits as a Libkern C++ object. OSNumber objects are mutable: you can add to or set their values.

**Use Restrictions**

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSNumber provides no concurrency protection; it's up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as IORegistryEntry, handle synchronization via defined member functions for setting properties.

## Topics

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

withNumber(const char *, unsigned int)

Creates and initializes an instance of OSNumber with an unsigned integer value represented as a C string.

withNumber(unsigned long long, unsigned int)

Creates and initializes an instance of OSNumber with an integer value.

### Instance Methods

- addValue

- free

- getMetaClass

- init

- init

- isEqualTo

Compares the number with an OSNumber.

- isEqualTo

Compares the string with an OSObject

- numberOfBits

Returns the number of bits the OSNumber was created with.

- numberOfBytes

- serialize

- setValue

- unsigned16BitValue

Returns the value of the OSNumber as a uint16_t value.

- unsigned32BitValue

Returns the value of the OSNumber as a uint32_t value.

- unsigned64BitValue

Returns the value of the OSNumber as a uint64_t value.

- unsigned8BitValue

Returns the value of the OSNumber as a uint8_t value.

### Type Methods

+ withNumber

+ withNumber

## Relationships

### Inherits From

- OSObject

## See Also

### Simple Types

OSBoolean

OSBoolean wraps a boolean value in a C++ object for use in Libkern collections.

OSString

OSString wraps a C string in a C++ object for use in Libkern collections.

OSData

OSData wraps an array of bytes in a C++ object for use in Libkern collections.


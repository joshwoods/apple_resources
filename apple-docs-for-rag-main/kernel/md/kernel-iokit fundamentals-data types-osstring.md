

- Kernel
- IOKit Fundamentals
- Data Types
-  OSString 

Class

# OSString

OSString wraps a C string in a C++ object for use in Libkern collections.

macOS 10.0+

``` source
class OSString : OSObject
```

## Overview

OSString is a container class for managing arrays of characters. An OSString normally maintains its own character buffer and allows changes, but you can create an "immutable" OSString that references an external C string buffer using the "NoCopy" creator functions. Functions called to change the contents of an immutable OSString will fail.

**Encodings**

OSString makes no provisions for different character encodings and assumes that a string is a nul-terminated sequence of single-byte characters. User-space code must either assume an encoding (typically ASCII or UTF-8) or determine it in some other way (such as an IORegistryEntry property).

**Altering Strings**

OSString's intended use is as a reference-counted object container for a C string and little more. While OSString provides full access to the underlying C string, it provides little in the way of string object manipulation; there are no append or insert functions, only a set-character function. If you need to manipulate OSStrings, it's generally best to get the C strings, alter them as necessary, and create a new OSString object from the resulting C string.

**Use Restrictions**

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSString provides no concurrency protection; it's up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as IORegistryEntry, handle synchronization via defined member functions for setting properties.

## Topics

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

### Instance Methods

- free

- getCStringNoCopy

Returns a pointer to the OSString object’s internal data buffer.

- getChar

- getLength

Returns length of string not including null terminator.

- getMetaClass

- initWithCString

- initWithCStringNoCopy

- initWithString

- isEqualTo

Compares the string with an OSString.

- isEqualTo

Compares the string with an OSData.

- isEqualTo

Compares the string with a c-string.

- isEqualTo

Compares the string with an OSObject

- serialize

- setChar

### Type Methods

+ withCString

Allocates an OSString object with a copy of a c-string.

+ withCString

Allocates an OSString object with a copy of a c-string, up to a given length.

+ withCStringNoCopy

Allocates an OSString object with a copy of a c-string.

+ withString

Allocates an OSString object with a copy of an OString object.

## Relationships

### Inherits From

- OSObject

## See Also

### Simple Types

OSBoolean

OSBoolean wraps a boolean value in a C++ object for use in Libkern collections.

OSNumber

OSNumber wraps an integer value in a C++ object for use in Libkern collections.

OSData

OSData wraps an array of bytes in a C++ object for use in Libkern collections.


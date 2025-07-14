

- Kernel
- IOKit Fundamentals
- Data Types
-  OSData 

Class

# OSData

OSData wraps an array of bytes in a C++ object for use in Libkern collections.

macOS 10.0+

``` source
class OSData : OSObject
```

## Overview

OSData represents an array of bytes as a Libkern C++ object. OSData objects are mutable: You can add bytes to them and overwrite portions of the byte array.

**Use Restrictions**

With very few exceptions in the I/O Kit, all Libkern-based C++ classes, functions, and macros are **unsafe** to use in a primary interrupt context. Consult the I/O Kit documentation related to primary interrupts for more information.

OSData provides no concurrency protection; it's up to the usage context to provide any protection necessary. Some portions of the I/O Kit, such as IORegistryEntry, handle synchronization via defined member functions for setting properties.

## Topics

### Miscellaneous

appendByte

Appends a single byte value to the OSData object's internal data buffer a specified number of times.

appendBytes(const OSData *)

Appends the data contained in another OSData object.

appendBytes(const void *, unsigned int)

Appends a buffer of bytes to the OSData object's internal data buffer.

ensureCapacity

Ensures the array has enough space to store the requested number of bytes.

free

Deallocates or releases any resources used by the OSDictionary instance.

getBytesNoCopy()

Returns a pointer to the OSData object's internal data buffer.

getBytesNoCopy(unsigned int, unsigned int)

Returns a pointer into the OSData object's internal data buffer with a given offset and length.

getCapacity

Returns the total number of bytes the OSData can store without reallocating.

getCapacityIncrement

Returns the storage increment of the OSData object.

getLength

Returns the number of bytes in or referenced by the OSData object.

initWithBytes

Initializes an instance of OSData with a copy of the provided data buffer.

initWithBytesNoCopy

Initializes an instance of OSData to share the provided data buffer.

initWithCapacity

Initializes an instance of OSData.

initWithData(const OSData *)

Creates and initializes an instance of OSData with contents copied from another OSData object.

initWithData(const OSData *, unsigned int, unsigned int)

Initializes an instance of OSData with contents copied from a range within another OSData object.

isEqualTo(const OSData *)

Tests the equality of two OSData objects.

isEqualTo(const OSMetaClassBase *)

Tests the equality of an OSData object to an arbitrary object.

isEqualTo(const OSString *)

Tests the equality of an OSData object to an OSString.

isEqualTo(const void *, unsigned int)

Tests the equality of an OSData object's contents to a C array of bytes.

serialize

Archives the receiver into the provided OSSerialize object.

setCapacityIncrement

Sets the storage increment of the array.

withBytes

Creates and initializes an instance of OSData with a copy of the provided data buffer.

withBytesNoCopy

Creates and initializes an instance of OSData that shares the provided data buffer.

withCapacity

Creates and initializes an empty instance of OSData.

withData(const OSData *)

Creates and initializes an instance of OSData with contents copied from another OSData object.

withData(const OSData *, unsigned int, unsigned int)

Creates and initializes an instance of OSData with contents copied from a range within another OSData object.

### Instance Methods

- appendByte

- appendBytes

- appendBytes

Appends a buffer of bytes to the OSData object’s internal data buffer.

- ensureCapacity

- free

- getBytesNoCopy

Returns a pointer to the OSData object’s internal data buffer.

- getBytesNoCopy

Returns a pointer to the OSData object’s internal data buffer.

- getCapacity

Returns length of preallocated capacity.

- getCapacityIncrement

- getLength

Returns length of data present.

- getMetaClass

- initWithBytes

- initWithBytesNoCopy

- initWithCapacity

- initWithData

- initWithData

- isEqualTo

Compares the data with an OSData

- isEqualTo

Compares the data with an OSString

- isEqualTo

Compares the data with a pointer to bytes

- isEqualTo

Compares the data with an OSObject

- isSerializable

- serialize

- setCapacityIncrement

- setDeallocFunction

- setSerializable

### Type Methods

+ withBytes

+ withBytesNoCopy

+ withCapacity

Allocates an OSData object with preallocated capacity.

+ withData

Allocates an OSData object with a copy of bytes from another OSData.

+ withData

Allocates an OSData object with a copy of bytes from a subset of another OSData.

## Relationships

### Inherits From

- OSObject

## See Also

### Simple Types

OSBoolean

OSBoolean wraps a boolean value in a C++ object for use in Libkern collections.

OSString

OSString wraps a C string in a C++ object for use in Libkern collections.

OSNumber

OSNumber wraps an integer value in a C++ object for use in Libkern collections.


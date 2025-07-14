

- DriverKit
-  OSData 

Class

# OSData

A container for untyped data.

DriverKitiOSiPadOSmacOS

``` source
class OSData;
```

## Overview

OSData represents an array of bytes as a container object. OSData objects are mutable: You can add bytes to them and overwrite portions of the byte array.

OSData provides no concurrency protection; it’s up to the usage context to provide any protection necessary.

## Topics

### Creating a Data Object

withBytes

Allocates an OSData object with a copy of bytes.

withBytesNoCopy

Allocates an OSData object with a copy of bytes.

withCapacity

Allocates an OSData object with preallocated capacity.

withData

Allocates an OSData object with a copy of bytes from another OSData.

withData

Allocates an OSData object with a copy of bytes from a subset of another OSData.

OSDataCreate

OSDataPtr

free

### Getting Bytes

getBytesNoCopy

Returns a pointer to the OSData object’s internal data buffer.

getBytesNoCopy

Returns a pointer to the OSData object’s internal data buffer.

OSDataGetBytes

OSDataGetBytesPtr

### Appending Data to the Object

appendBytes

Appends a buffer of bytes to the OSData object’s internal data buffer.

appendBytes

Appends a buffer of bytes to the OSData object’s internal data buffer.

appendBytes

Appends a buffer of bytes to the OSData object’s internal data buffer.

OSDataAppendBytes

### Inspecting a Data Object

getCapacity

Returns length of preallocated capacity.

getLength

Returns length of data present.

OSDataGetLength

### Comparing Data Objects

isEqualTo

Compares the data with an OSData

isEqualTo

Compares the data with an OSObject

isEqualTo

Compares the data with an OSString

isEqualTo

Compares the data with a pointer to bytes

## Relationships

### Inherits From

- OSContainer

## See Also

### Registry data types

OSArray

A container for an ordered, random-access collection of objects.

OSDictionary

A container for a collection with elements that are key-value pairs.

OSBoolean

A container for a true or false value.

OSNumber

A container for an integer value.

OSString

A container for managing an array of characters.

OSSerialization

A container for one or more objects, serialized in a binary data format that is suitable for messaging.

OSCollection

The base class for DriverKit collection objects.

OSContainer

The base class for DriverKit data objects.

OSObject

The base class for DriverKit objects

OSSymbol

A container for managing an array of characters.

IOFixed

A fixed-point number.


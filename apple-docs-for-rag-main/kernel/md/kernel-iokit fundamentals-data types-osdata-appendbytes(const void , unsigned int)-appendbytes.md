

- Kernel
- IOKit Fundamentals
- Data Types
- OSData
-  appendBytes(const void \*, unsigned int) 

# appendBytes(const void \*, unsigned int)

Appends a buffer of bytes to the OSData object's internal data buffer.

``` source
virtual bool appendBytes( 
 const void *bytes, 
 unsigned intnumBytes); 
```

## Parameters 

`bytes`  

A pointer to the data to append. If `bytes` is `NULL` then a zero-filled buffer of length `numBytes` is appended.

`numBytes`  

The number of bytes from `bytes` to append.

## Return Value

`true` if the new data was successfully added, `false` on failure.

## Overview

This function immediately resizes the OSData's buffer, if necessary, to accommodate the new total size.

An OSData object created "NoCopy" does not allow bytes to be appended.

## See Also

### Miscellaneous

appendByte

Appends a single byte value to the OSData object's internal data buffer a specified number of times.

appendBytes(const OSData *)

Appends the data contained in another OSData object.

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


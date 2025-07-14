

- Kernel
- IOKit Fundamentals
- Data Types
- OSData
-  withBytesNoCopy 

# withBytesNoCopy

Creates and initializes an instance of OSData that shares the provided data buffer.

``` source
static OSData * withBytesNoCopy( 
 void *bytes, 
 unsigned intnumBytes); 
```

## Parameters 

`bytes`  

The buffer of data to represent.

`numBytes`  

The length of `bytes`.

## Return Value

A instance of OSData that shares the provided byte array, with a reference count of 1; `NULL on failure. `

## Overview

An OSData object created with this function does not claim ownership of the data buffer, but shares it with the caller. When the caller determines that the OSData object has actually been freed, it can safely dispose of the data buffer. Conversely, if it frees the shared data buffer, it must not attempt to use the OSData object and should release it.

An OSData object created with shared external data cannot append bytes, but you can get the byte pointer and modify bytes within the shared buffer.

## See Also

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

withCapacity

Creates and initializes an empty instance of OSData.

withData(const OSData *)

Creates and initializes an instance of OSData with contents copied from another OSData object.

withData(const OSData *, unsigned int, unsigned int)

Creates and initializes an instance of OSData with contents copied from a range within another OSData object.


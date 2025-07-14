

- DriverKit
- OSData
-  withBytesNoCopy 

Static Method

# withBytesNoCopy

Allocates an OSData object with a copy of bytes.

DriverKitiOSiPadOSmacOS

``` source
static OSDataPtr withBytesNoCopy(void * bytes, size_t numBytes);
```

## Parameters 

`bytes`  

C-pointer to untyped data. The data will be copied at the time of the call.

`numBytes`  

Count of bytes to be copied.

## Return Value

NULL on failure, otherwise the allocated OSData with reference count 1 to be released by the caller.

## Discussion

Allocates an OSData object with a copy of bytes. A synonym for OSData::withBytes() for compatibility with kernel code.

## See Also

### Creating a Data Object

withBytes

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


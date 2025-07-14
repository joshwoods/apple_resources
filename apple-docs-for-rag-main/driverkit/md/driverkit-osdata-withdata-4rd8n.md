

- DriverKit
- OSData
-  withData 

Static Method

# withData

Allocates an OSData object with a copy of bytes from a subset of another OSData.

DriverKitiOSiPadOSmacOS

``` source
static OSDataPtr withData(const OSData * inData, size_t start, size_t numBytes);
```

## Parameters 

`inData`  

An OSData object to copy. The data will be copied at the time of the call.

`start`  

An offset into the OSData object to copy from.

`numBytes`  

The length of data to copy. If (start + numBytes) exceeds the length of inData, the call will fail.

## Return Value

NULL on failure, otherwise the allocated OSData with reference count 1 to be released by the caller.

## See Also

### Creating a Data Object

withBytes

Allocates an OSData object with a copy of bytes.

withBytesNoCopy

Allocates an OSData object with a copy of bytes.

withCapacity

Allocates an OSData object with preallocated capacity.

withData

Allocates an OSData object with a copy of bytes from another OSData.

OSDataCreate

OSDataPtr

free


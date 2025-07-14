

- DriverKit
- OSData
-  withCapacity 

Static Method

# withCapacity

Allocates an OSData object with preallocated capacity.

DriverKitiOSiPadOSmacOS

``` source
static OSDataPtr withCapacity(uint32_t capacity);
```

## Parameters 

`capacity`  

Number of bytes of data the object can hold.

## Return Value

NULL on failure, otherwise the allocated OSData with reference count 1 to be released by the caller.

## Discussion

Allocates an OSData object with preallocated capacity. The OSData will have zero length until data is added to it with appendBytes().

## See Also

### Creating a Data Object

withBytes

Allocates an OSData object with a copy of bytes.

withBytesNoCopy

Allocates an OSData object with a copy of bytes.

withData

Allocates an OSData object with a copy of bytes from another OSData.

withData

Allocates an OSData object with a copy of bytes from a subset of another OSData.

OSDataCreate

OSDataPtr

free




- DriverKit
- OSData
-  getBytesNoCopy 

Instance Method

# getBytesNoCopy

Returns a pointer to the OSData object’s internal data buffer.

DriverKitiOSiPadOSmacOS

``` source
const void * getBytesNoCopy(size_t start, size_t numBytes) const;
```

## Parameters 

`start`  

An offset into the OSData object.

`numBytes`  

The length of data intended to be read. If (start + numBytes) exceeds the size of the OSData’s length, the call will fail.

## Return Value

A pointer to the data or NULL if the OSData does not have data for all the requested range.

## See Also

### Getting Bytes

getBytesNoCopy

Returns a pointer to the OSData object’s internal data buffer.

OSDataGetBytes

OSDataGetBytesPtr


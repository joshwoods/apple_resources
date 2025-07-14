

- DriverKit
- OSData
-  getBytesNoCopy 

Instance Method

# getBytesNoCopy

Returns a pointer to the OSData object’s internal data buffer.

DriverKitiOSiPadOSmacOS

``` source
const void * getBytesNoCopy() const;
```

## Return Value

A pointer to the data or NULL if the OSData has zero length.

## See Also

### Getting Bytes

getBytesNoCopy

Returns a pointer to the OSData object’s internal data buffer.

OSDataGetBytes

OSDataGetBytesPtr


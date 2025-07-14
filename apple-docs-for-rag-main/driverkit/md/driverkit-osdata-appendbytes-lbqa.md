

- DriverKit
- OSData
-  appendBytes 

Instance Method

# appendBytes

Appends a buffer of bytes to the OSData object’s internal data buffer.

DriverKitiOSiPadOSmacOS

``` source
bool appendBytes(const void * bytes, size_t numBytes);
```

## Parameters 

`bytes`  

C-pointer to untyped data. The data will be copied at the time of the call.

`numBytes`  

Count of bytes to be copied.

## Return Value

True on success or false on failure, due to allocation failure.

## See Also

### Appending Data to the Object

appendBytes

Appends a buffer of bytes to the OSData object’s internal data buffer.

OSDataAppendBytes


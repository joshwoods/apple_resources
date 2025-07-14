

- DriverKit
- OSString
-  getCStringNoCopy 

Instance Method

# getCStringNoCopy

Returns a pointer to the OSString object’s internal data buffer.

DriverKitiOSiPadOSmacOS

``` source
const char * getCStringNoCopy() const;
```

## Return Value

A pointer to the string or NULL if the OSString has zero length. The string will be null terminated.

## See Also

### Getting a C String

OSStringGetStringPtr

OSStringPtr


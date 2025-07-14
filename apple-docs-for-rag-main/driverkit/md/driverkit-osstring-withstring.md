

- DriverKit
- OSString
-  withString 

Static Method

# withString

Allocates an OSString object with a copy of an OString object.

DriverKitiOSiPadOSmacOS

``` source
static OSStringPtr withString(const OSString * aString);
```

## Parameters 

`aString`  

OSString object to copy from. The string will be copied at the time of the call.

## Return Value

NULL on failure, otherwise the allocated OSString with reference count 1 to be released by the caller.

## Discussion

Allocates an OSString object with a copy of an OString object.

## See Also

### Creating a String

withCString

Allocates an OSString object with a copy of a c-string.

withCString

Allocates an OSString object with a copy of a c-string, up to a given length.

withCStringNoCopy

Allocates an OSString object with a copy of a c-string.

OSStringCreate

free




- DriverKit
- OSString
-  withCStringNoCopy 

Static Method

# withCStringNoCopy

Allocates an OSString object with a copy of a c-string.

DriverKitiOSiPadOSmacOS

``` source
static OSStringPtr withCStringNoCopy(const char * cString);
```

## Parameters 

`cString`  

Pointer to null terminated c-string. The string will be copied at the time of the call.

## Return Value

NULL on failure, otherwise the allocated OSString with reference count 1 to be released by the caller.

## Discussion

Allocates an OSString object with a copy of a c-string. A synonym for OSString::withCString() for compatibility with kernel code.

## See Also

### Creating a String

withString

Allocates an OSString object with a copy of an OString object.

withCString

Allocates an OSString object with a copy of a c-string.

withCString

Allocates an OSString object with a copy of a c-string, up to a given length.

OSStringCreate

free


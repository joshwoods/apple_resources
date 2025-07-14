

- DriverKit
- OSString
-  withCString 

Static Method

# withCString

Allocates an OSString object with a copy of a c-string, up to a given length.

DriverKitiOSiPadOSmacOS

``` source
static OSStringPtr withCString(const char * cString, size_t length);
```

## Parameters 

`cString`  

Pointer to null terminated c-string. The string will be copied at the time of the call.

`length`  

Maximum length of the string to copy.

## Return Value

NULL on failure, otherwise the allocated OSString with reference count 1 to be released by the caller.

## See Also

### Creating a String

withString

Allocates an OSString object with a copy of an OString object.

withCString

Allocates an OSString object with a copy of a c-string.

withCStringNoCopy

Allocates an OSString object with a copy of a c-string.

OSStringCreate

free


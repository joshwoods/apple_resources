

- DriverKit
- OSNumber
-  withNumber 

Static Method

# withNumber

Allocates an OSNumber object with value from a c-string and size.

DriverKitiOSiPadOSmacOS

``` source
static OSNumberPtr withNumber(const char * valueString, size_t numberOfBits);
```

## Parameters 

`valueString`  

A c-string which will be parsed with strtoll(,,0).

`numberOfBits`  

Size of the value. Only 8, 16, 32, or 64 are valid sizes.

## Return Value

NULL on failure, otherwise the allocated OSNumber with reference count 1 to be released by the caller.

## Discussion

Allocates an OSNumber object with value from a c-string and size.

## See Also

### Creating a Number Object

withNumber

Allocates an OSNumber object with value and size.

OSNumberCreateWithUInt64Value

free

OSNumberPtr


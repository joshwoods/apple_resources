

- Core Services
- Carbon Core
- Carbon Core Functions
-  UTCreateStringForOSType(\_:) Deprecated

Function

# UTCreateStringForOSType(\_:)

Encodes an `OSType` into a string suitable for use as a tag argument.

macOS 10.3–12.0Deprecated

``` source
func UTCreateStringForOSType(_ inOSType: OSType) -> Unmanaged
```

## Parameters 

`inOSType`  

The `OSType` to convert.

## Return Value

A string that encodes the OSType.

## Discussion

The UTI functions assume that all alternate identifier tags can be represented as Core Foundation strings. OSTypes are integer-based rather than string-based, so to pass an OSType into a UTI function, you must call this function to convert it to a string.

## See Also

### Related Documentation

func UTGetOSTypeFromString(CFString) -> OSType

Decodes a tag string into an OSType.




- Core Services
- Carbon Core
- Carbon Core Functions
-  UTGetOSTypeFromString(\_:) Deprecated

Function

# UTGetOSTypeFromString(\_:)

Decodes a tag string into an OSType.

macOS 10.3–12.0Deprecated

``` source
func UTGetOSTypeFromString(_ inString: CFString) -> OSType
```

## Parameters 

`inString`  

A string that encodes an OSType.

## Return Value

The OSType that was encoded in the string.

## Discussion

You call this function to convert an OSType string returned by a UTI function back into the integer-based OSType.

## See Also

### Related Documentation

func UTCreateStringForOSType(OSType) -> Unmanaged&lt;CFString>

Encodes an `OSType` into a string suitable for use as a tag argument.


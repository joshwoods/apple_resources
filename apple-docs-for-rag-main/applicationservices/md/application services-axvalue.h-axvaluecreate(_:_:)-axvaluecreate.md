

- Application Services
- AXValue.h
-  AXValueCreate(\_:\_:) 

Function

# AXValueCreate(\_:\_:)

macOS 10.2+

``` source
func AXValueCreate(
    _ theType: AXValueType,
    _ valuePtr: UnsafeRawPointer
) -> AXValue?
```

## Parameters 

`theType`  

`valuePtr`  

## Discussion

Encodes a structure pointed to by valuePtr into a CFTypeRef.

## See Also

### Miscellaneous

func AXValueGetType(AXValue) -> AXValueType

func AXValueGetTypeID() -> CFTypeID

func AXValueGetValue(AXValue, AXValueType, UnsafeMutableRawPointer) -> Bool


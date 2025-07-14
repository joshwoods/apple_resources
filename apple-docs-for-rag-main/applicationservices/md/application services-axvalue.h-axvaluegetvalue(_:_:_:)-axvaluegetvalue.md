

- Application Services
- AXValue.h
-  AXValueGetValue(\_:\_:\_:) 

Function

# AXValueGetValue(\_:\_:\_:)

macOS 10.2+

``` source
func AXValueGetValue(
    _ value: AXValue,
    _ theType: AXValueType,
    _ valuePtr: UnsafeMutableRawPointer
) -> Bool
```

## Parameters 

`value`  

## Discussion

Decodes the structure stored in value and copies it into valuePtr. If the structure stored in value is not the same as requested by theType, the function returns false.

## See Also

### Miscellaneous

func AXValueCreate(AXValueType, UnsafeRawPointer) -> AXValue?

func AXValueGetType(AXValue) -> AXValueType

func AXValueGetTypeID() -> CFTypeID


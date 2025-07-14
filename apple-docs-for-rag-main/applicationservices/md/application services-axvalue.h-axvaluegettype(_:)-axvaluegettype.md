

- Application Services
- AXValue.h
-  AXValueGetType(\_:) 

Function

# AXValueGetType(\_:)

macOS 10.2+

``` source
func AXValueGetType(_ value: AXValue) -> AXValueType
```

## Parameters 

`value`  

## Discussion

Returns the structure type encoded in value. If the type is not recognized, it returns kAXValueIllegalType.

## See Also

### Miscellaneous

func AXValueCreate(AXValueType, UnsafeRawPointer) -> AXValue?

func AXValueGetTypeID() -> CFTypeID

func AXValueGetValue(AXValue, AXValueType, UnsafeMutableRawPointer) -> Bool


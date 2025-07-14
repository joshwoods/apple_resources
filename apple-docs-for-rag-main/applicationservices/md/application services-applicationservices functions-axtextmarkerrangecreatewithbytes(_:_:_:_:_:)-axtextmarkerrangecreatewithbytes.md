

- Application Services
- ApplicationServices Functions
-  AXTextMarkerRangeCreateWithBytes(\_:\_:\_:\_:\_:) 

Function

# AXTextMarkerRangeCreateWithBytes(\_:\_:\_:\_:\_:)

macOS 12.0+

``` source
func AXTextMarkerRangeCreateWithBytes(
    _ allocator: CFAllocator?,
    _ startMarkerBytes: UnsafePointer,
    _ startMarkerLength: CFIndex,
    _ endMarkerBytes: UnsafePointer,
    _ endMarkerLength: CFIndex
) -> AXTextMarkerRange
```


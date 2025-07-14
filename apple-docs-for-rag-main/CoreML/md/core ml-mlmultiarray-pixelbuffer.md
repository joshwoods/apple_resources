

- Core ML
- MLMultiArray
-  pixelBuffer 

Instance Property

# pixelBuffer

A reference to the multiarray’s underlying pixel buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var pixelBuffer: CVPixelBuffer? { get }
```

## See Also

### Accessing a Multiarray’s Elements

subscript(Int) -> NSNumber

Accesses the multiarray by using a linear offset.

subscript([NSNumber]) -> NSNumber

Accesses the multiarray by using a number array that has an element for each dimension.

var dataPointer: UnsafeMutableRawPointer

A pointer to the multiarray’s underlying memory.

Deprecated


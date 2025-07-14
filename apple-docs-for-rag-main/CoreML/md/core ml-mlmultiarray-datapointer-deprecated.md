

- Core ML
- MLMultiArray
-  dataPointer Deprecated

Instance Property

# dataPointer

A pointer to the multiarray’s underlying memory.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1+macOS 10.13–11.0DeprecatedtvOS 11.0+visionOS 1.0–2.4DeprecatedwatchOS 4.0–9.0Deprecated

``` source
var dataPointer: UnsafeMutableRawPointer { get }
```

Deprecated

Use getBytesWithHandler or getMutableBytesWithHandler instead. For Swift, use withUnsafeBytes or withUnsafeMutableBytes.

## See Also

### Accessing a Multiarray’s Elements

subscript(Int) -> NSNumber

Accesses the multiarray by using a linear offset.

subscript([NSNumber]) -> NSNumber

Accesses the multiarray by using a number array that has an element for each dimension.

var pixelBuffer: CVPixelBuffer?

A reference to the multiarray’s underlying pixel buffer.


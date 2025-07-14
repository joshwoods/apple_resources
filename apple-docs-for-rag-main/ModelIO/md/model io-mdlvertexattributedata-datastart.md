

- Model I/O
- MDLVertexAttributeData
-  dataStart 

Instance Property

# dataStart

The offset, in bytes, from the start of the data to where vertex attribute information begins.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var dataStart: UnsafeMutableRawPointer { get set }
```

## See Also

### Accessing Data for a Vertex Attribute

var stride: Int

The stride, in bytes, between vertex information for consecutive vertices in the data.

var format: MDLVertexFormat

The format of per-vertex data for the attribute.




- Metal
- MTLAccelerationStructureTriangleGeometryDescriptor
-  indexType 

Instance Property

# indexType

The data type of indices in the index buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var indexType: MTLIndexType { get set }
```

## Discussion

The data type must be MTLDataType.ushort or MTLDataType.uint. The default is MTLDataType.uint.

## See Also

### Specifying Index Data

var indexBuffer: (any MTLBuffer)?

A buffer that contains indices for the vertices that compose the triangle list.

var indexBufferOffset: Int

The offset, in bytes, to the first index in the buffer.


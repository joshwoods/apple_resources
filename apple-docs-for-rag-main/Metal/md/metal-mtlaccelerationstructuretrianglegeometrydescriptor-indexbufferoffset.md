

- Metal
- MTLAccelerationStructureTriangleGeometryDescriptor
-  indexBufferOffset 

Instance Property

# indexBufferOffset

The offset, in bytes, to the first index in the buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var indexBufferOffset: Int { get set }
```

## Discussion

Specify an offset that is a multiple of the index data type size and a multiple of the platform’s buffer offset alignment.

## See Also

### Specifying Index Data

var indexBuffer: (any MTLBuffer)?

A buffer that contains indices for the vertices that compose the triangle list.

var indexType: MTLIndexType

The data type of indices in the index buffer.


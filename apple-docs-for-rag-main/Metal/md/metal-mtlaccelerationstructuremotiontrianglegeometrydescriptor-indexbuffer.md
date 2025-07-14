

- Metal
- MTLAccelerationStructureMotionTriangleGeometryDescriptor
-  indexBuffer 

Instance Property

# indexBuffer

A buffer that contains indices for the vertices that compose the triangle list.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var indexBuffer: (any MTLBuffer)? { get set }
```

## Discussion

This property can be `nil`, in which case the vertex data defines the triangle list implicitly. You must store indices in a packed data format.

## See Also

### Specifying Index Data

var indexType: MTLIndexType

The data type of indices in the index buffer.

var indexBufferOffset: Int

The offset, in bytes, to the first index in the buffer.


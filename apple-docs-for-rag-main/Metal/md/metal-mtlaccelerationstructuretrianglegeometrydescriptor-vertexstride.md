

- Metal
- MTLAccelerationStructureTriangleGeometryDescriptor
-  vertexStride 

Instance Property

# vertexStride

The stride, in bytes, between vertices in the vertex buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var vertexStride: Int { get set }
```

## Discussion

The stride must be at least 12 bytes and must be a multiple of 4 bytes. The default value is 12 bytes.

## See Also

### Specifying Vertex Data

var vertexBuffer: (any MTLBuffer)?

A buffer that contains vertex data.

var vertexBufferOffset: Int

The offset, in bytes, for the first vertex in the vertex buffer.


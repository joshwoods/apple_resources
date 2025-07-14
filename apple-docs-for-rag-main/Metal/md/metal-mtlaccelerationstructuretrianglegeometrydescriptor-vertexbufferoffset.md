

- Metal
- MTLAccelerationStructureTriangleGeometryDescriptor
-  vertexBufferOffset 

Instance Property

# vertexBufferOffset

The offset, in bytes, for the first vertex in the vertex buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var vertexBufferOffset: Int { get set }
```

## Discussion

The vertex must be a multiple of the vertex stride and must be a multiple of 4 bytes. The default value is 0.

## See Also

### Specifying Vertex Data

var vertexBuffer: (any MTLBuffer)?

A buffer that contains vertex data.

var vertexStride: Int

The stride, in bytes, between vertices in the vertex buffer.


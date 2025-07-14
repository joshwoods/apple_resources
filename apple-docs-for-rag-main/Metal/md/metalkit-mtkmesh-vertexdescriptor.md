

- MetalKit
- MTKMesh
-  vertexDescriptor 

Instance Property

# vertexDescriptor

A Model I/O vertex descriptor specifying the data layout in the vertex buffers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var vertexDescriptor: MDLVertexDescriptor { get }
```

## Discussion

This is a convenience property. The MTKMesh class does not use this descriptor, but your application may use this object to determine rendering state or create a MTLVertexDescriptor object to build a MTLRenderPipelineState object capable of interpreting the data in vertexBuffers.

## See Also

### Vertex Properties

var vertexBuffers: [MTKMeshBuffer]

An array of buffers in which mesh vertex data resides.

var vertexCount: Int

The number of vertices in the vertex buffers.


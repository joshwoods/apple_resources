

- MetalKit
- MTKSubmesh
-  mesh 

Instance Property

# mesh

The parent mesh containing the vertex data of this submesh.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
weak var mesh: MTKMesh? { get }
```

## Discussion

The buffer of this parent mesh should be set in the encoder before a call to drawIndexedPrimitives(type:indexCount:indexType:indexBuffer:indexBufferOffset:) is made.


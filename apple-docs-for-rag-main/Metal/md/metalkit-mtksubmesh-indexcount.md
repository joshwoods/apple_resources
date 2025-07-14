

- MetalKit
- MTKSubmesh
-  indexCount 

Instance Property

# indexCount

The number of indices in the index buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var indexCount: Int { get }
```

## Discussion

Use this value for the `indexCount` parameter in a call to drawIndexedPrimitives(type:indexCount:indexType:indexBuffer:indexBufferOffset:).

## See Also

### Properties used to Draw Indexed Primitives

var indexBuffer: MTKMeshBuffer

The index buffer used to render the submesh object.

var indexType: MTLIndexType

The type of index data in the index buffer.

var primitiveType: MTLPrimitiveType

The primitive type with which to draw the submesh object.


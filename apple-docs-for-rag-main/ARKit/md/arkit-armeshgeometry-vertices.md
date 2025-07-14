

- ARKit
- ARMeshGeometry
-  vertices 

Instance Property

# vertices

The vertices of the mesh.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
var vertices: ARGeometrySource { get }
```

## Discussion

The count equals the total number of vertices. Since each vertex is the type `SIMD3`, componentsPerVector is three.

The following code demonstrates retrieving a vertex at a particular index.

```
extension ARMeshGeometry { 
    func vertex(at index: UInt32) -> SIMD3 {
        assert(vertices.format == MTLVertexFormat.float3, "Expected three floats (twelve bytes) per vertex.")
        let vertexPointer = vertices.buffer.contents().advanced(by: vertices.offset + (vertices.stride * Int(index)))
        let vertex = vertexPointer.assumingMemoryBound(to: SIMD3.self).pointee
        return vertex
    }
}
```

## See Also

### Accessing Geometry Data

class ARGeometrySource

Mesh data in a buffer-based array.


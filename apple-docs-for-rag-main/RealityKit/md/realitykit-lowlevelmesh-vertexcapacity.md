

- RealityKit
- LowLevelMesh
-  vertexCapacity 

Instance Property

# vertexCapacity

The capacity of the vertex buffer, measured in vertices.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
var vertexCapacity: Int { get }
```

## Discussion

This value is equivalent to vertexCapacity.

## See Also

### Describing a low-level mesh

let descriptor: LowLevelMesh.Descriptor

The definition of the structure of this low-level mesh.

var parts: LowLevelMesh.PartsCollection

A mutable collection of parts.

var indexCapacity: Int

The capacity of the index buffer, measured in indices.


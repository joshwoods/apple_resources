

- RealityKit
- LowLevelMesh
-  indexCapacity 

Instance Property

# indexCapacity

The capacity of the index buffer, measured in indices.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
var indexCapacity: Int { get }
```

## Discussion

This value is equivalent to indexCapacity.

## See Also

### Describing a low-level mesh

let descriptor: LowLevelMesh.Descriptor

The definition of the structure of this low-level mesh.

var parts: LowLevelMesh.PartsCollection

A mutable collection of parts.

var vertexCapacity: Int

The capacity of the vertex buffer, measured in vertices.


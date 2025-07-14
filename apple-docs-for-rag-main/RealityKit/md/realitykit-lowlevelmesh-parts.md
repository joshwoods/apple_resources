

- RealityKit
- LowLevelMesh
-  parts 

Instance Property

# parts

A mutable collection of parts.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
var parts: LowLevelMesh.PartsCollection { get set }
```

## Discussion

The parts of a LowLevelMesh object specify how to interpret the index buffer. You can also use `parts` to customize the material index and primitive type.

## See Also

### Describing a low-level mesh

let descriptor: LowLevelMesh.Descriptor

The definition of the structure of this low-level mesh.

var indexCapacity: Int

The capacity of the index buffer, measured in indices.

var vertexCapacity: Int

The capacity of the vertex buffer, measured in vertices.


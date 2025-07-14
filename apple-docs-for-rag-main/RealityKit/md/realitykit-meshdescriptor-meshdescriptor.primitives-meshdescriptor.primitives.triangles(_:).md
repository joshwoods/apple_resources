

- RealityKit
- MeshDescriptor
- MeshDescriptor.Primitives
-  MeshDescriptor.Primitives.triangles(\_:) 

Case

# MeshDescriptor.Primitives.triangles(\_:)

Defines one or more triangles with an integer array of indices.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case triangles([UInt32])
```

## Discussion

Add three vertex index integers per triangle. For example, you can represent a single triangle with three indices.

```
.triangles([0, 1, 2])
```


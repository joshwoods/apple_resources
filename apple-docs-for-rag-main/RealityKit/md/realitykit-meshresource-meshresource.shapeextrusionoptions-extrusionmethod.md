

- RealityKit
- MeshResource
- MeshResource.ShapeExtrusionOptions
-  extrusionMethod 

Instance Property

# extrusionMethod

Specifies the extrusion type applied to the swept shape in 3D space.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var extrusionMethod: MeshResource.ShapeExtrusionOptions.ExtrusionMethod
```

## Discussion

For example, use `.linear(depth: 0.25)` to extrude the shape in Z by 0.25 meters.


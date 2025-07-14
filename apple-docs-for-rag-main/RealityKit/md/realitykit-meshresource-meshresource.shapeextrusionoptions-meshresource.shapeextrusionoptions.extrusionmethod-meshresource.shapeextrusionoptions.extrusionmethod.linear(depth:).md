

- RealityKit
- MeshResource
- MeshResource.ShapeExtrusionOptions
- MeshResource.ShapeExtrusionOptions.ExtrusionMethod
-  MeshResource.ShapeExtrusionOptions.ExtrusionMethod.linear(depth:) 

Case

# MeshResource.ShapeExtrusionOptions.ExtrusionMethod.linear(depth:)

Extrudes the shape with a linear extrusion in Z by the desired depth.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case linear(depth: Float)
```

## Discussion

For example an extrusion that has a linear depth of 0.6 meters:

```
var extrusionOptions = ShapeExtrusionOptions()
extrusionOptions.extrusionMethod = .linear(depth: 0.6)
```

You can also use MeshResource.ShapeExtrusionOptions.ExtrusionMethod.tracePositions(_:) an equivalent way.

```
.tracePositions([
    [0, 0, -depth/2],
    [0, 0,  depth/2]
)
```


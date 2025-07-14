

- RealityKit
- MeshResource
- MeshResource.ShapeExtrusionOptions
- MeshResource.ShapeExtrusionOptions.MaterialAssignment
-  init(front:back:extrusion:frontChamfer:backChamfer:) 

Initializer

# init(front:back:extrusion:frontChamfer:backChamfer:)

Creates a material assignment structure with options for each side of an extruded shape.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    front: UInt32 = 0,
    back: UInt32 = 0,
    extrusion: UInt32 = 0,
    frontChamfer: UInt32 = 0,
    backChamfer: UInt32 = 0
)
```

## Parameters 

`front`  

The material index for the front face of the shape.

`back`  

The material index for the back face of the shape.

`extrusion`  

The material index for the extruded faces of the shape.

`frontChamfer`  

The material index for the chamfered edges between the front and sides of the shape.

`backChamfer`  

The material index for the chamfered edges between the back and sides of the shape.

## Discussion

The default for any omitted parameter is `0`.


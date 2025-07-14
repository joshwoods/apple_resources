

- SceneKit
- SCNPhysicsShape
-  init(geometry:options:) 

Initializer

# init(geometry:options:)

Creates a physics shape based on a geometry object.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init(
    geometry: SCNGeometry,
    options: [SCNPhysicsShape.Option : Any]? = nil
)
```

## Parameters 

`geometry`  

A geometry object.

`options`  

A dictionary of options affecting the level of detail of the physics shape, or `nil` to use default options. For applicable keys and their possible values, see `Shape Creation Options Keys`.

## Return Value

A new physics shape object.

## Discussion

If you create a physics shape using one of the basic geometry classes (SCNBox, SCNSphere, SCNPyramid, SCNCone, SCNCylinder, or SCNCapsule), SceneKit uses an idealized form of that geometry for the physics shape instead of using the geometry’s vertex data to simulate collisions. For example, if you create a physics shape from an SCNSphere object, SceneKit simulates collisions for any object that passes within the sphere’s radius.

Because the idealized forms of simple geometries are computationally much simpler than the vertex data needed for displaying them, using basic geometries for physics shapes (or compound shapes created from basic geometries with the init(shapes:transforms:) method) often provides the best balance between simulation accuracy and performance.

To use the newly created physics shape, create a physics body with the the init(type:shape:) method, or assign the shape to the physicsShape property of an existing body.

## See Also

### Creating Physics Shapes

convenience init(node: SCNNode, options: [SCNPhysicsShape.Option : Any]?)

Creates a physics shape from a node or hierarchy of nodes.


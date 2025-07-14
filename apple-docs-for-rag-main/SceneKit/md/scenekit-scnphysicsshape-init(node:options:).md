

- SceneKit
- SCNPhysicsShape
-  init(node:options:) 

Initializer

# init(node:options:)

Creates a physics shape from a node or hierarchy of nodes.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init(
    node: SCNNode,
    options: [SCNPhysicsShape.Option : Any]? = nil
)
```

## Parameters 

`node`  

A node object. The node must contain an SCNGeometry object in its geometry property or have one or more child (or descendant) nodes that contain geometry.

`options`  

A dictionary of options affecting the level of detail of the physics shape, or `nil` to use default options. For applicable keys and their possible values, see `Shape Creation Options Keys`.

## Return Value

A new physics shape object.

## Discussion

To use the newly created physics shape, create a physics body with the the init(type:shape:) method, or assign the shape to the physicsShape property of an existing body.

The node used to create the physics shape need not be the same as the node whose physics body you attach the shape to—or even be in the scene whose physics world you use the shape in. For example, you can create a physics body for a complex object by building a hierarchy of nodes containing simple geometries (using the SCNBox and SCNSphere classes), and then creating a physics shape from those nodes. The resulting physics shape, a compound of bounding boxes or convex hulls, provides a rough approximation of the complex object without a high cost to simulation performance.

## See Also

### Creating Physics Shapes

convenience init(geometry: SCNGeometry, options: [SCNPhysicsShape.Option : Any]?)

Creates a physics shape based on a geometry object.


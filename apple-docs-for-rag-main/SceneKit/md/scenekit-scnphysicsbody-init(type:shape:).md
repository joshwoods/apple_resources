

- SceneKit
- SCNPhysicsBody
-  init(type:shape:) 

Initializer

# init(type:shape:)

Creates a physics body with the specified type and shape.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init(
    type: SCNPhysicsBodyType,
    shape: SCNPhysicsShape?
)
```

## Parameters 

`type`  

A constant that determines how a body responds to forces and collisions. See SCNPhysicsBodyType.

`shape`  

A physics shape defining the volume of the body for collision detection purposes.

## Return Value

A new physics body object.

## Discussion

For the body to participate in collision detection or respond to forces, you must attach it to the physicsBody property of an SCNNode object in a scene.

If you pass `nil` for the shape parameter, SceneKit automatically creates a physics shape for the body when you attach it to a node, based on that node’s geometry property. To create a physics shape that’s based on the geometries of a node and its hierarchy of children, or to control the level of detail in a physics shape, create the physics shape manually using an SCNPhysicsShape class method.

Note

For nodes containing custom geometry, the physics shape SceneKit automatically creates is a rough approximation of the geometry. This approximation, or *convex hull*, provides a compromise between accuracy and performance in collision detection. For the best collision detection performance, create an SCNPhysicsShape instance based on a basic geometry class (SCNBox, SCNSphere, SCNPyramid, SCNCone, SCNCylinder, or SCNCapsule).

## See Also

### Related Documentation

var type: SCNPhysicsBodyType

A constant that determines how the physics body responds to forces and collisions.

var physicsShape: SCNPhysicsShape?

An object that defines the solid volume of the physics body for use in collision detection.

### Creating Physics Bodies

class func `static`() -> Self

Creates a physics body that is unaffected by forces or collisions and that cannot move.

class func dynamic() -> Self

Creates a physics body that can be affected by forces and collisions.

class func kinematic() -> Self

Creates a physics body that is unaffected by forces or collisions but that can cause collisions affecting other bodies when moved.


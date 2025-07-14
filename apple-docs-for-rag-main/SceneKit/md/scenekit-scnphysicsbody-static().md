

- SceneKit
- SCNPhysicsBody
-  static() 

Type Method

# static()

Creates a physics body that is unaffected by forces or collisions and that cannot move.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func `static`() -> Self
```

## Return Value

A new physics body object.

## Discussion

Use static bodies to construct fixtures in your scene that other bodies need to collide with but that do not themselves move, such as floors, walls, and terrain.

For the body to participate in collision detection or respond to forces, you must attach it to the physicsBody property of an SCNNode object in a scene.

SceneKit automatically creates a physics shape for the body when you attach it to a node, based on that node’s geometry property. To create a physics shape that’s based on the geometries of a node and its hierarchy of children, or to control the level of detail in a physics shape, create the physics shape manually using an SCNPhysicsShape class method.

Note

For nodes containing custom geometry, the physics shape SceneKit automatically creates is a rough approximation of the geometry. This approximation, or *convex hull*, provides a compromise between accuracy and performance in collision detection. For the best collision detection performance, create an SCNPhysicsShape instance based on a basic geometry class (SCNBox, SCNSphere, SCNPyramid, SCNCone, SCNCylinder, or SCNCapsule).

## See Also

### Related Documentation

var type: SCNPhysicsBodyType

A constant that determines how the physics body responds to forces and collisions.

var physicsShape: SCNPhysicsShape?

An object that defines the solid volume of the physics body for use in collision detection.

### Creating Physics Bodies

convenience init(type: SCNPhysicsBodyType, shape: SCNPhysicsShape?)

Creates a physics body with the specified type and shape.

class func dynamic() -> Self

Creates a physics body that can be affected by forces and collisions.

class func kinematic() -> Self

Creates a physics body that is unaffected by forces or collisions but that can cause collisions affecting other bodies when moved.


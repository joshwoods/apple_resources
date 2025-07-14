

- SceneKit
-  SCNPhysicsShape 

Class

# SCNPhysicsShape

An abstraction of a physics body’s solid volume for tuning collision detection.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNPhysicsShape
```

## Overview

When SceneKit performs contact detection and other simulations for the SCNPhysicsBody objects in your scene, it uses physics shapes instead of the rendered geometry of visible objects. This approach both improves simulation performance and allows you to more easily design your gameplay around scene elements the player can interact with.

### Simple Versus Complex Shapes

When you allow SceneKit to automatically create a physics shape, it uses the simplest possible shape roughly matching the geometry of the node the physics body is attached to. This approach maximizes simulation performance but can lead to unrealistic physics behavior for some objects.

You can make the simulation behave more realistically by defining physics shapes that more closely follow the visible geometry in your scene. This approach comes at a cost to performance, so you want to limit the amount of detail in your physics shapes. Use the highest levels of detail only on bodies for which precise collision detection is important for your app.

If you create a physics shape using one of the basic geometry classes (SCNBox, SCNSphere, SCNPyramid, SCNCone, SCNCylinder, or SCNCapsule), SceneKit uses an idealized form of that geometry for the physics shape instead of using the geometry’s vertex data to simulate collisions. For example, if you create a physics shape from an SCNSphere object, SceneKit simulates collisions for any object that passes within the sphere’s radius.

Because the idealized forms of simple geometries are computationally much simpler than the vertex data needed for displaying them, using basic geometries for physics shapes (or compound shapes created from basic geometries with the init(shapes:transforms:) method) often provides the best balance between simulation accuracy and performance.

### Changing a Physics Body’s Shape

Physics shapes are immutable, but you can change the shape associated with a physics body by creating a new SCNPhysicsShape instance and assigning it to the body’s physicsShape property.

## Topics

### Creating Physics Shapes

convenience init(geometry: SCNGeometry, options: [SCNPhysicsShape.Option : Any]?)

Creates a physics shape based on a geometry object.

convenience init(node: SCNNode, options: [SCNPhysicsShape.Option : Any]?)

Creates a physics shape from a node or hierarchy of nodes.

### Combining Physics Shapes

convenience init(shapes: [SCNPhysicsShape], transforms: [NSValue]?)

Creates a new physics shape by combining others.

### Getting Information About a Shape

var sourceObject: Any

The object that was used to create the shape.

var options: [SCNPhysicsShape.Option : Any]?

The options dictionary that was used to create the shape.

var transforms: [NSValue]?

The array of transforms that was used to create a compound shape.

### Shape Options

struct Option

Keys for the options dictionary used when creating a physics shape.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Physics Bodies

class SCNPhysicsBody

The physics simulation attributes attached to a scene graph node.


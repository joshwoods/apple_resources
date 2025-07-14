

- SceneKit
- SCNPhysicsBody
-  continuousCollisionDetectionThreshold 

Instance Property

# continuousCollisionDetectionThreshold

The minimum distance the body must travel for SceneKit to apply a more precise (but more costly) algorithm to detect contacts with other bodies.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var continuousCollisionDetectionThreshold: CGFloat { get set }
```

## Discussion

SceneKit’s physics engine can employ two kinds of collision detection:

- With *discrete* collision detection, when SceneKit simulates physics before rendering each frame (see timeStep and SCNSceneRendererDelegate), it updates the position of each physics body based on the body’s velocity during that time interval, then checks to see whether the body at its new position intersects other bodies.

- With *continuous* collision detection, SceneKit calculates the volume that will be traversed by a body during each frame, then checks to see whether that volume intersects other bodies.

This property’s value defaults to `0.0`, resulting in discrete collision detection at all times. When this value is nonzero, SceneKit applies continuous collision whenever the body travels more than the specified distance within one timeStep.

Discrete collision detection offers high performance, but can lead to inaccurate results for small, fast-moving bodies. Continuous collision detection has a performance cost and works only for spherical physics shapes, but provides more accurate results.

For example, in a game involving projectiles and targets, a small projectile may pass through a target if it moves farther than the target’s thickness within one time step. By setting the projectile’s continuousCollisionDetectionThreshold to match its diameter, you ensure that SceneKit always detects collisions between the projectile and other objects.

## See Also

### Working with Contacts and Collisions

var categoryBitMask: Int

A mask that defines which categories this physics body belongs to.

var contactTestBitMask: Int

A mask that defines which categories of bodies cause intersection notifications with this physics body.

var collisionBitMask: Int

A mask that defines which categories of physics bodies can collide with this physics body.

struct SCNPhysicsCollisionCategory

Default values for a physics body’s categoryBitMask and collisionBitMask properties.


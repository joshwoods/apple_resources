

- SceneKit
- SCNPhysicsBody
-  collisionBitMask 

Instance Property

# collisionBitMask

A mask that defines which categories of physics bodies can collide with this physics body.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var collisionBitMask: Int { get set }
```

## Discussion

When two physics bodies contact each other, a collision may occur. SceneKit compares the body’s collision mask to the other body’s category mask by performing a bitwise AND operation. If the result is a nonzero value, then the body is affected by the collision. Each body independently chooses whether it wants to be affected by the other body. For example, you might choose to avoid collision calculations that would make negligible changes to a body’s velocity.

The default value is all (a bit mask whose every bit is enabled), specifying that the body will collide with bodies of all other categories.

## See Also

### Working with Contacts and Collisions

var categoryBitMask: Int

A mask that defines which categories this physics body belongs to.

var contactTestBitMask: Int

A mask that defines which categories of bodies cause intersection notifications with this physics body.

struct SCNPhysicsCollisionCategory

Default values for a physics body’s categoryBitMask and collisionBitMask properties.

var continuousCollisionDetectionThreshold: CGFloat

The minimum distance the body must travel for SceneKit to apply a more precise (but more costly) algorithm to detect contacts with other bodies.


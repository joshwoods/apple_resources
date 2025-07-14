

- SpriteKit
- SKPhysicsBody
-  collisionBitMask 

Instance Property

# collisionBitMask

A mask that defines which categories of physics bodies can collide with this physics body.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var collisionBitMask: UInt32 { get set }
```

## Mentioned in 

About Collisions and Contacts

## Discussion

When two physics bodies contact each other, a collision may occur. This body’s collision mask is compared to the other body’s category mask by performing a logical AND operation. If the result is a nonzero value, this body is affected by the collision. Each body independently chooses whether it wants to be affected by the other body. For example, you might use this to avoid collision calculations that would make negligible changes to a body’s velocity.

The default value is `0xFFFFFFFF` (all bits set).

## See Also

### Working with Collisions and Contacts

About Collisions and Contacts

Learn how to set up nodes for collision detection.

var categoryBitMask: UInt32

A mask that defines which categories this physics body belongs to.

var usesPreciseCollisionDetection: Bool

A Boolean value that determines whether the physics world uses an iterative collision detection algorithm.

var contactTestBitMask: UInt32

A mask that defines which categories of physics bodies cause intersection notifications with this physics body.

func allContactedBodies() -> [SKPhysicsBody]

The physics bodies that this physics body is in contact with.


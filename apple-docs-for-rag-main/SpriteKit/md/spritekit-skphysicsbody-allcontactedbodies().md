

- SpriteKit
- SKPhysicsBody
-  allContactedBodies() 

Instance Method

# allContactedBodies()

The physics bodies that this physics body is in contact with.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func allContactedBodies() -> [SKPhysicsBody]
```

## Return Value

An array of SKPhysicsBody objects that this body is in contact with.

## See Also

### Working with Collisions and Contacts

About Collisions and Contacts

Learn how to set up nodes for collision detection.

var categoryBitMask: UInt32

A mask that defines which categories this physics body belongs to.

var collisionBitMask: UInt32

A mask that defines which categories of physics bodies can collide with this physics body.

var usesPreciseCollisionDetection: Bool

A Boolean value that determines whether the physics world uses an iterative collision detection algorithm.

var contactTestBitMask: UInt32

A mask that defines which categories of physics bodies cause intersection notifications with this physics body.


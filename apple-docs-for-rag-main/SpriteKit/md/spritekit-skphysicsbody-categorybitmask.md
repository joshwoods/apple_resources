

- SpriteKit
- SKPhysicsBody
-  categoryBitMask 

Instance Property

# categoryBitMask

A mask that defines which categories this physics body belongs to.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var categoryBitMask: UInt32 { get set }
```

## Mentioned in 

About Collisions and Contacts

## Discussion

Every physics body in a scene can be assigned to up to 32 different categories, each corresponding to a bit in the bit mask. You define the mask values used in your game. In conjunction with the collisionBitMask and contactTestBitMask properties, you define which physics bodies interact with each other and when your game is notified of these interactions.

The default value is `0xFFFFFFFF` (all bits set).

## See Also

### Working with Collisions and Contacts

About Collisions and Contacts

Learn how to set up nodes for collision detection.

var collisionBitMask: UInt32

A mask that defines which categories of physics bodies can collide with this physics body.

var usesPreciseCollisionDetection: Bool

A Boolean value that determines whether the physics world uses an iterative collision detection algorithm.

var contactTestBitMask: UInt32

A mask that defines which categories of physics bodies cause intersection notifications with this physics body.

func allContactedBodies() -> [SKPhysicsBody]

The physics bodies that this physics body is in contact with.


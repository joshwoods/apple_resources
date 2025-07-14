

- SpriteKit
- SKPhysicsBody
-  usesPreciseCollisionDetection 

Instance Property

# usesPreciseCollisionDetection

A Boolean value that determines whether the physics world uses an iterative collision detection algorithm.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var usesPreciseCollisionDetection: Bool { get set }
```

## Discussion

When SpriteKit performs collision detection, it first determines the locations of all of the physics bodies in the scene. Then it determines whether collisions or contacts occurred. This computational method is fast, but can sometimes result in missed collisions. A small body might move so fast that it completely passes through another physics body without ever having a frame of animation where the two touch each other.

If you have physics bodies that must collide, you can hint to SpriteKit to use a more precise collision model to check for interactions. This model is more expensive, so it should be used sparingly. When either body uses precise collisions, multiple contact iterations are evaluated to ensure that all contacts are detected.

The default value is false. If two bodies in a collision do not perform precise collision detection, and one passes completely through the other in a single frame, no collision is detected. If this property is set to true on either body, the simulation performs a more precise and more expensive calculation to detect these collisions. This property should be set to true on small, fast moving bodies.

## See Also

### Working with Collisions and Contacts

About Collisions and Contacts

Learn how to set up nodes for collision detection.

var categoryBitMask: UInt32

A mask that defines which categories this physics body belongs to.

var collisionBitMask: UInt32

A mask that defines which categories of physics bodies can collide with this physics body.

var contactTestBitMask: UInt32

A mask that defines which categories of physics bodies cause intersection notifications with this physics body.

func allContactedBodies() -> [SKPhysicsBody]

The physics bodies that this physics body is in contact with.




- SceneKit
- SCNPhysicsBody
-  categoryBitMask 

Instance Property

# categoryBitMask

A mask that defines which categories this physics body belongs to.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var categoryBitMask: Int { get set }
```

## Discussion

Every physics body in a scene can be assigned to one or more categories, each corresponding to a bit in the bit mask. You define the mask values used in your game. Use this property together with the physicsShape and contactTestBitMask properties to define which physics bodies interact with each other and when your game is notified of interactions.

The default value is static for static bodies and default for dynamic and kinematic bodies.

## See Also

### Working with Contacts and Collisions

var contactTestBitMask: Int

A mask that defines which categories of bodies cause intersection notifications with this physics body.

var collisionBitMask: Int

A mask that defines which categories of physics bodies can collide with this physics body.

struct SCNPhysicsCollisionCategory

Default values for a physics body’s categoryBitMask and collisionBitMask properties.

var continuousCollisionDetectionThreshold: CGFloat

The minimum distance the body must travel for SceneKit to apply a more precise (but more costly) algorithm to detect contacts with other bodies.


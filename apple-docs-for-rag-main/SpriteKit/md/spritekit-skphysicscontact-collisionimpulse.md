

- SpriteKit
- SKPhysicsContact
-  collisionImpulse 

Instance Property

# collisionImpulse

The impulse that specifies how hard these two bodies struck each other in Newton-seconds.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var collisionImpulse: CGFloat { get }
```

## See Also

### Inspecting the Contact Properties

var bodyA: SKPhysicsBody

The first body in the contact.

var bodyB: SKPhysicsBody

The second body in the contact.

var contactPoint: CGPoint

The contact point between the two physics bodies, in scene coordinates.

var contactNormal: CGVector

The normal vector specifying the direction of the collision.


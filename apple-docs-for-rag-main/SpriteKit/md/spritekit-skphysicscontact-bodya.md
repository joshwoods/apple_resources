

- SpriteKit
- SKPhysicsContact
-  bodyA 

Instance Property

# bodyA

The first body in the contact.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var bodyA: SKPhysicsBody { get }
```

## See Also

### Inspecting the Contact Properties

var bodyB: SKPhysicsBody

The second body in the contact.

var contactPoint: CGPoint

The contact point between the two physics bodies, in scene coordinates.

var collisionImpulse: CGFloat

The impulse that specifies how hard these two bodies struck each other in Newton-seconds.

var contactNormal: CGVector

The normal vector specifying the direction of the collision.


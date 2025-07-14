

- SpriteKit
- SKPhysicsContact
-  contactPoint 

Instance Property

# contactPoint

The contact point between the two physics bodies, in scene coordinates.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var contactPoint: CGPoint { get }
```

## See Also

### Inspecting the Contact Properties

var bodyA: SKPhysicsBody

The first body in the contact.

var bodyB: SKPhysicsBody

The second body in the contact.

var collisionImpulse: CGFloat

The impulse that specifies how hard these two bodies struck each other in Newton-seconds.

var contactNormal: CGVector

The normal vector specifying the direction of the collision.




- SpriteKit
- SKPhysicsBody
-  affectedByGravity 

Instance Property

# affectedByGravity

A Boolean value that indicates whether this physics body is affected by the physics world’s gravity.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var affectedByGravity: Bool { get set }
```

## Discussion

The physics world’s gravity property defines the gravitational forces applied to volume-based bodies in the scene.

The default value is `true`. This property is ignored on edge-based bodies, which are always unaffected by gravity.

Physics bodies with `affectedByGravity` set to `false` are still affected by the gravity fields created by linearGravityField(withVector:) and radialGravityField().

## See Also

### Defining How Forces Affect a Physics Body

var allowsRotation: Bool

A Boolean value that indicates whether the physics body is affected by angular forces and impulses applied to it.

var isDynamic: Bool

A Boolean value that indicates whether the physics body is moved by the physics simulation.




- SpriteKit
- SKPhysicsBody
-  allowsRotation 

Instance Property

# allowsRotation

A Boolean value that indicates whether the physics body is affected by angular forces and impulses applied to it.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var allowsRotation: Bool { get set }
```

## Discussion

The default value is true. This property is ignored on edge-based bodies, which are unaffected by forces in the system.

## See Also

### Defining How Forces Affect a Physics Body

var affectedByGravity: Bool

A Boolean value that indicates whether this physics body is affected by the physics world’s gravity.

var isDynamic: Bool

A Boolean value that indicates whether the physics body is moved by the physics simulation.


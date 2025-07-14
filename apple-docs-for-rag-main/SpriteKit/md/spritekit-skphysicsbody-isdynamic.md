

- SpriteKit
- SKPhysicsBody
-  isDynamic 

Instance Property

# isDynamic

A Boolean value that indicates whether the physics body is moved by the physics simulation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isDynamic: Bool { get set }
```

## Mentioned in 

Getting Started with Spring Joints

Getting Started with Physics Bodies

## Discussion

The default value is true. If the value is false, the physics body ignores all forces and impulses applied to it. This property is ignored on edge-based bodies; they are automatically static.

## See Also

### Defining How Forces Affect a Physics Body

var affectedByGravity: Bool

A Boolean value that indicates whether this physics body is affected by the physics world’s gravity.

var allowsRotation: Bool

A Boolean value that indicates whether the physics body is affected by angular forces and impulses applied to it.


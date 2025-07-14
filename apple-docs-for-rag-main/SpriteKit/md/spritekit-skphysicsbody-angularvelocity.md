

- SpriteKit
- SKPhysicsBody
-  angularVelocity 

Instance Property

# angularVelocity

The physics body’s angular speed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var angularVelocity: CGFloat { get set }
```

## Mentioned in 

Making Physics Bodies Move

## Discussion

The angular velocity is a pseudo vector around an axis vector of `(0.0,0.0,1.0)` measured in radians per second.

## See Also

### Inspecting a Physics Body’s Position and Velocity

var velocity: CGVector

The physics body’s velocity vector, measured in meters per second.

var isResting: Bool

A Boolean property that indicates whether the object is at rest within the physics simulation.


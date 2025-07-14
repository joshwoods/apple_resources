

- SpriteKit
- SKPhysicsBody
-  isResting 

Instance Property

# isResting

A Boolean property that indicates whether the object is at rest within the physics simulation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isResting: Bool { get set }
```

## Discussion

This property is automatically set to true by the physics simulation when it determines that the body is at rest. This means that the body is at rest on another body in the system. Resting bodies do not participate in the physics simulation until an impulse is applied to the object or another object collides with it. This improves the performance of the physics simulation. If all bodies in the world are resting, the entire simulation is at rest, reducing the number of calculations that are performed by the physics world.

## See Also

### Inspecting a Physics Body’s Position and Velocity

var velocity: CGVector

The physics body’s velocity vector, measured in meters per second.

var angularVelocity: CGFloat

The physics body’s angular speed.


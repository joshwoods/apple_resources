

- SceneKit
- SCNPhysicsBody
-  restitution 

Instance Property

# restitution

A factor that determines how much kinetic energy the body loses or gains in collisions.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var restitution: CGFloat { get set }
```

## Discussion

This property simulates the “bounciness” of a body. A restitution of `1.0` means that the body loses no energy in a collision—for example, a ball dropped onto a flat surface will bounce back to the height it fell from. A restitution of `0.0` means the body does not bounce after a collision. A restitution of greater than `1.0` causes the body to gain energy in collisions. The default restitution is `0.5`.

## See Also

### Defining a Body’s Physical Properties

var mass: CGFloat

The mass of the body, in kilograms.

var charge: CGFloat

The electric charge of the body, in coulombs.

var friction: CGFloat

The body’s resistance to sliding motion.

var rollingFriction: CGFloat

The body’s resistance to rolling motion.

var damping: CGFloat

A factor that reduces the body’s linear velocity.

var angularDamping: CGFloat

A factor that reduces the body’s angular velocity.

var momentOfInertia: SCNVector3

The body’s moment of inertia, expressed in the local coordinate system of the node that contains the body.

var usesDefaultMomentOfInertia: Bool

A Boolean value that determines whether SceneKit automatically calculates the body’s moment of inertia or allows setting a custom value.

var centerOfMassOffset: SCNVector3

The position of the body’s center of mass relative to its local coordinate origin.


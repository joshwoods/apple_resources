

- SceneKit
- SCNPhysicsBody
-  damping 

Instance Property

# damping

A factor that reduces the body’s linear velocity.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var damping: CGFloat { get set }
```

## Discussion

This property simulates the effect of fluid friction or air resistance on a body. A damping factor of `0.0` specifies no loss in velocity, and a damping factor of `1.0` prevents the body from moving. The default damping factor is `0.1`.

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

var restitution: CGFloat

A factor that determines how much kinetic energy the body loses or gains in collisions.

var angularDamping: CGFloat

A factor that reduces the body’s angular velocity.

var momentOfInertia: SCNVector3

The body’s moment of inertia, expressed in the local coordinate system of the node that contains the body.

var usesDefaultMomentOfInertia: Bool

A Boolean value that determines whether SceneKit automatically calculates the body’s moment of inertia or allows setting a custom value.

var centerOfMassOffset: SCNVector3

The position of the body’s center of mass relative to its local coordinate origin.




- SceneKit
- SCNPhysicsBody
-  rollingFriction 

Instance Property

# rollingFriction

The body’s resistance to rolling motion.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var rollingFriction: CGFloat { get set }
```

## Discussion

This property simulates the traction between a rounded body and bodies it might roll against. A rolling friction of `0.0` (the default) means that a body induced to roll (for example, by being placed on an inclined surface) will continue to roll without slowing down unless otherwise acted upon, and a rolling friction of `1.0` prevents the body from rolling.

## See Also

### Defining a Body’s Physical Properties

var mass: CGFloat

The mass of the body, in kilograms.

var charge: CGFloat

The electric charge of the body, in coulombs.

var friction: CGFloat

The body’s resistance to sliding motion.

var restitution: CGFloat

A factor that determines how much kinetic energy the body loses or gains in collisions.

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




- SceneKit
- SCNPhysicsBody
-  friction 

Instance Property

# friction

The body’s resistance to sliding motion.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var friction: CGFloat { get set }
```

## Discussion

This property simulates the roughness of the body’s surface. When two bodies are in contact and a force is applied that would cause them to slide against one another, the friction values for both bodies determine their resistance to motion. If both bodies’ friction value is `0.0`, they slide freely against each other. If both bodies’ friction value is `1.0`, they do not slide at all. The default friction is `0.5`.

## See Also

### Defining a Body’s Physical Properties

var mass: CGFloat

The mass of the body, in kilograms.

var charge: CGFloat

The electric charge of the body, in coulombs.

var rollingFriction: CGFloat

The body’s resistance to rolling motion.

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


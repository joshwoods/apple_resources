

- SceneKit
- SCNPhysicsBody
-  usesDefaultMomentOfInertia 

Instance Property

# usesDefaultMomentOfInertia

A Boolean value that determines whether SceneKit automatically calculates the body’s moment of inertia or allows setting a custom value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var usesDefaultMomentOfInertia: Bool { get set }
```

## Discussion

A body’s moment of inertia determines how it responds to torques (that is, forces with a rotational component).

If this property is true (the default), SceneKit automatically determines the body’s moment of inertia based on its shape and mass. Set this property to false and use the momentOfInertia property to define a custom moment of inertia (for example, to model an object of non-uniform density).

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

var damping: CGFloat

A factor that reduces the body’s linear velocity.

var angularDamping: CGFloat

A factor that reduces the body’s angular velocity.

var momentOfInertia: SCNVector3

The body’s moment of inertia, expressed in the local coordinate system of the node that contains the body.

var centerOfMassOffset: SCNVector3

The position of the body’s center of mass relative to its local coordinate origin.


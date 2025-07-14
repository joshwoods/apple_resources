

- SceneKit
- SCNPhysicsBody
-  momentOfInertia 

Instance Property

# momentOfInertia

The body’s moment of inertia, expressed in the local coordinate system of the node that contains the body.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var momentOfInertia: SCNVector3 { get set }
```

## Discussion

A body’s moment of inertia determines how it responds to torques (that is, forces with a rotational component). Each component of this vector is the moment of inertia for the corresponding principal axis (in the coordinate system containing the physics body). For example, if the x-component value of the moment vector is less than the y-component value, the body rotates more freely about its x-axis than its y-axis.

By default, SceneKit automatically determines the body’s moment of inertia based on its shape and mass. Use this property to define a custom moment of inertia (for example, to model an object of non-uniform density). Using a custom moment of inertia requires setting the usesDefaultMomentOfInertia property to false.

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

var usesDefaultMomentOfInertia: Bool

A Boolean value that determines whether SceneKit automatically calculates the body’s moment of inertia or allows setting a custom value.

var centerOfMassOffset: SCNVector3

The position of the body’s center of mass relative to its local coordinate origin.


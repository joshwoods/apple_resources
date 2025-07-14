

- Core Animation
- CASpringAnimation
-  mass 

Instance Property

# mass

The mass of the object attached to the end of the spring.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var mass: CGFloat { get set }
```

## Discussion

The default mass is `1`. Increasing this value will increase the spring effect: the attached object will be subject to more oscillations and greater overshoot, resulting in an increased settlingDuration. Decreasing the mass will reduce the spring effect: there will be fewer oscillations and a reduced overshoot, resulting in a decreased settlingDuration.

## See Also

### Configuring Physical Attributes

var damping: CGFloat

Defines how the spring’s motion should be damped due to the forces of friction.

var initialVelocity: CGFloat

The initial velocity of the object attached to the spring.

var settlingDuration: CFTimeInterval

The estimated duration required for the spring system to be considered at rest.

var stiffness: CGFloat

The spring stiffness coefficient.


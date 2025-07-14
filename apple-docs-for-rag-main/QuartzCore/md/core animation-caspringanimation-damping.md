

- Core Animation
- CASpringAnimation
-  damping 

Instance Property

# damping

Defines how the spring’s motion should be damped due to the forces of friction.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var damping: CGFloat { get set }
```

## Discussion

The default value of the damping property is `10`. Reducing this value reduces the energy loss with each oscillation: the animated value will overshoot the toValue and the settlingDuration may be greater than the duration. Increasing the value increases the energy loss with each duration: there will be fewer and smaller oscillations and the settlingDuration may be smaller than the duration.

## See Also

### Configuring Physical Attributes

var initialVelocity: CGFloat

The initial velocity of the object attached to the spring.

var mass: CGFloat

The mass of the object attached to the end of the spring.

var settlingDuration: CFTimeInterval

The estimated duration required for the spring system to be considered at rest.

var stiffness: CGFloat

The spring stiffness coefficient.


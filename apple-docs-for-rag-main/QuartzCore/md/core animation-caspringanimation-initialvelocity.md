

- Core Animation
- CASpringAnimation
-  initialVelocity 

Instance Property

# initialVelocity

The initial velocity of the object attached to the spring.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var initialVelocity: CGFloat { get set }
```

## Discussion

Defaults to `0`, which represents an unmoving object. Negative values represent the object moving away from the spring attachment point, positive values represent the object moving towards the spring attachment point.

## See Also

### Configuring Physical Attributes

var damping: CGFloat

Defines how the spring’s motion should be damped due to the forces of friction.

var mass: CGFloat

The mass of the object attached to the end of the spring.

var settlingDuration: CFTimeInterval

The estimated duration required for the spring system to be considered at rest.

var stiffness: CGFloat

The spring stiffness coefficient.


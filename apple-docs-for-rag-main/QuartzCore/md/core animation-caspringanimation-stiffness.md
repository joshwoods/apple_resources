

- Core Animation
- CASpringAnimation
-  stiffness 

Instance Property

# stiffness

The spring stiffness coefficient.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var stiffness: CGFloat { get set }
```

## Discussion

The default stiffness coefficient is `100`. Increasing the stiffness reduces the number of oscillations and will reduce the settling duration. Decreasing the stiffness increases the the number of oscillations and will increase the settling duration.

## See Also

### Configuring Physical Attributes

var damping: CGFloat

Defines how the spring’s motion should be damped due to the forces of friction.

var initialVelocity: CGFloat

The initial velocity of the object attached to the spring.

var mass: CGFloat

The mass of the object attached to the end of the spring.

var settlingDuration: CFTimeInterval

The estimated duration required for the spring system to be considered at rest.


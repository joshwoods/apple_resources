

- Core Animation
- CASpringAnimation
-  settlingDuration 

Instance Property

# settlingDuration

The estimated duration required for the spring system to be considered at rest.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var settlingDuration: CFTimeInterval { get }
```

## Discussion

The duration is evaluated for the current animation parameters and may not the same as the duration.

The following code creates a spring animation with a duration of 2 seconds.

```
let spring = CASpringAnimation()

spring.keyPath = "position.x"
spring.fromValue = 0
spring.toValue = 640
spring.damping = 5
spring.duration = 2
```

With a damping coefficient of `5`, the settling duration is approximately 2.85 seconds: the animated layer bounces around the target position several times before settling. However, changing the damping property to `15` reduces the settling duration to just over 1 second: the animated layer quickly comes to a stop as it reaches the target position.

All of the spring animation’s physical attributes: damping, initialVelocity, mass and stiffness, can affect the settling duration.

## See Also

### Configuring Physical Attributes

var damping: CGFloat

Defines how the spring’s motion should be damped due to the forces of friction.

var initialVelocity: CGFloat

The initial velocity of the object attached to the spring.

var mass: CGFloat

The mass of the object attached to the end of the spring.

var stiffness: CGFloat

The spring stiffness coefficient.




- SwiftUI
- Spring
-  init(duration:bounce:) 

Initializer

# init(duration:bounce:)

Creates a spring with the specified duration and bounce.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    duration: TimeInterval = 0.5,
    bounce: Double = 0.0
)
```

## Parameters 

`duration`  

Defines the pace of the spring. This is approximately equal to the settling duration, but for springs with very large bounce values, will be the duration of the period of oscillation for the spring.

`bounce`  

How bouncy the spring should be. A value of 0 indicates no bounces (a critically damped spring), positive values indicate increasing amounts of bounciness up to a maximum of 1.0 (corresponding to undamped oscillation), and negative values indicate overdamped springs with a minimum value of -1.0.

## See Also

### Creating a spring

init(mass: Double, stiffness: Double, damping: Double, allowOverDamping: Bool)

Creates a spring with the specified mass, stiffness, and damping.

init(response: Double, dampingRatio: Double)

Creates a spring with the specified response and damping ratio.

init(settlingDuration: TimeInterval, dampingRatio: Double, epsilon: Double)

Creates a spring with the specified duration and damping ratio.


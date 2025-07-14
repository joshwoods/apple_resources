

- SwiftUI
- Spring
-  mass 

Instance Property

# mass

The mass of the object attached to the end of the spring.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var mass: Double { get }
```

## Discussion

The default mass is 1. Increasing this value will increase the spring’s effect: the attached object will be subject to more oscillations and greater overshoot, resulting in an increased settling duration. Decreasing the mass will reduce the spring effect: there will be fewer oscillations and a reduced overshoot, resulting in a decreased settling duration.

## See Also

### Getting spring characteristics

var bounce: Double

How bouncy the spring is.

var damping: Double

Defines how the spring’s motion should be damped due to the forces of friction.

var dampingRatio: Double

The amount of drag applied, as a fraction of the amount needed to produce critical damping.

var duration: TimeInterval

The perceptual duration, which defines the pace of the spring.

var response: Double

The stiffness of the spring, defined as an approximate duration in seconds.

var settlingDuration: TimeInterval

The estimated duration required for the spring system to be considered at rest.

var stiffness: Double

The spring stiffness coefficient.


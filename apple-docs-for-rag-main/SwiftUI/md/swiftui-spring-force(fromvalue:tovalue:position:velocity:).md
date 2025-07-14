

- SwiftUI
- Spring
-  force(fromValue:toValue:position:velocity:) 

Instance Method

# force(fromValue:toValue:position:velocity:)

Calculates the force upon the spring given a current position, velocity, and divisor from the starting and end values for the spring to travel.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func force(
    fromValue: V,
    toValue: V,
    position: V,
    velocity: V
) -> V where V : Animatable
```

## Discussion

This value is in units of the vector type per second squared.

## See Also

### Calculating forces and durations

func force&lt;V>(target: V, position: V, velocity: V) -> V

Calculates the force upon the spring given a current position, target, and velocity amount of change.

func settlingDuration&lt;V>(target: V, initialVelocity: V, epsilon: Double) -> TimeInterval

The estimated duration required for the spring system to be considered at rest.

func settlingDuration&lt;V>(fromValue: V, toValue: V, initialVelocity: V, epsilon: Double) -> TimeInterval

The estimated duration required for the spring system to be considered at rest.


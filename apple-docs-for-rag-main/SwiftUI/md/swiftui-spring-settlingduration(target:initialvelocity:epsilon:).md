

- SwiftUI
- Spring
-  settlingDuration(target:initialVelocity:epsilon:) 

Instance Method

# settlingDuration(target:initialVelocity:epsilon:)

The estimated duration required for the spring system to be considered at rest.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func settlingDuration(
    target: V,
    initialVelocity: V = .zero,
    epsilon: Double
) -> TimeInterval where V : VectorArithmetic
```

## Discussion

The epsilon value specifies the threshhold for how small all subsequent values need to be before the spring is considered to have settled.

## See Also

### Calculating forces and durations

func force&lt;V>(target: V, position: V, velocity: V) -> V

Calculates the force upon the spring given a current position, target, and velocity amount of change.

func force&lt;V>(fromValue: V, toValue: V, position: V, velocity: V) -> V

Calculates the force upon the spring given a current position, velocity, and divisor from the starting and end values for the spring to travel.

func settlingDuration&lt;V>(fromValue: V, toValue: V, initialVelocity: V, epsilon: Double) -> TimeInterval

The estimated duration required for the spring system to be considered at rest.


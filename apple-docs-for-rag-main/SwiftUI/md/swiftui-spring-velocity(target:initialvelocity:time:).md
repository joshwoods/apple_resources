

- SwiftUI
- Spring
-  velocity(target:initialVelocity:time:) 

Instance Method

# velocity(target:initialVelocity:time:)

Calculates the velocity of the spring at a given time given a target amount of change.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func velocity(
    target: V,
    initialVelocity: V = .zero,
    time: TimeInterval
) -> V where V : VectorArithmetic
```

## See Also

### Getting spring state

func value&lt;V>(target: V, initialVelocity: V, time: TimeInterval) -> V

Calculates the value of the spring at a given time given a target amount of change.

func value&lt;V>(fromValue: V, toValue: V, initialVelocity: V, time: TimeInterval) -> V

Calculates the value of the spring at a given time for a starting and ending value for the spring to travel.

func velocity&lt;V>(fromValue: V, toValue: V, initialVelocity: V, time: TimeInterval) -> V

Calculates the velocity of the spring at a given time given a starting and ending value for the spring to travel.


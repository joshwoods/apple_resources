

- SwiftUI
- Spring
-  value(fromValue:toValue:initialVelocity:time:) 

Instance Method

# value(fromValue:toValue:initialVelocity:time:)

Calculates the value of the spring at a given time for a starting and ending value for the spring to travel.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func value(
    fromValue: V,
    toValue: V,
    initialVelocity: V,
    time: TimeInterval
) -> V where V : Animatable
```

## See Also

### Getting spring state

func value&lt;V>(target: V, initialVelocity: V, time: TimeInterval) -> V

Calculates the value of the spring at a given time given a target amount of change.

func velocity&lt;V>(target: V, initialVelocity: V, time: TimeInterval) -> V

Calculates the velocity of the spring at a given time given a target amount of change.

func velocity&lt;V>(fromValue: V, toValue: V, initialVelocity: V, time: TimeInterval) -> V

Calculates the velocity of the spring at a given time given a starting and ending value for the spring to travel.


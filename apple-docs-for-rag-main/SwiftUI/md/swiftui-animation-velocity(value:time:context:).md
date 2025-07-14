

- SwiftUI
- Animation
-  velocity(value:time:context:) 

Instance Method

# velocity(value:time:context:)

Calculates the current velocity of the animation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func velocity(
    value: V,
    time: TimeInterval,
    context: AnimationContext
) -> V? where V : VectorArithmetic
```

## Return Value

The current velocity of the animation, or `nil` if the the velocity isn’t available.


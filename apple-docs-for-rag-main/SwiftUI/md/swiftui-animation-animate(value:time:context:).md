

- SwiftUI
- Animation
-  animate(value:time:context:) 

Instance Method

# animate(value:time:context:)

Calculates the current value of the animation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func animate(
    value: V,
    time: TimeInterval,
    context: inout AnimationContext
) -> V? where V : VectorArithmetic
```

## Return Value

The current value of the animation, or `nil` if the animation has finished.


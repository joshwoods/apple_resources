

- SwiftUI
- Animation
-  shouldMerge(previous:value:time:context:) 

Instance Method

# shouldMerge(previous:value:time:context:)

Returns a Boolean value that indicates whether the current animation should merge with a previous animation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func shouldMerge(
    previous: Animation,
    value: V,
    time: TimeInterval,
    context: inout AnimationContext
) -> Bool where V : VectorArithmetic
```


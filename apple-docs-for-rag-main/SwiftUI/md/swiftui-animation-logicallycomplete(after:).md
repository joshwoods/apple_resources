

- SwiftUI
- Animation
-  logicallyComplete(after:) 

Instance Method

# logicallyComplete(after:)

Causes the animation to report logical completion after the specified duration, if it has not already logically completed.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func logicallyComplete(after duration: TimeInterval) -> Animation
```

## Parameters 

`duration`  

The duration after which the animation should report that it is logically complete.

## Return Value

An animation that reports logical completion after the given duration.

## Discussion

Note that the indicated duration will not cause the animation to continue running after the base animation has fully completed.

If the animation is removed before the given duration is reached, logical completion will be reported immediately.


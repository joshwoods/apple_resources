

- SwiftUI
- Transaction
-  addAnimationCompletion(criteria:\_:) 

Instance Method

# addAnimationCompletion(criteria:\_:)

Adds a completion to run when the animations created with this transaction are all complete.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func addAnimationCompletion(
    criteria: AnimationCompletionCriteria = .logicallyComplete,
    _ completion: @escaping () -> Void
)
```

## Discussion

The completion callback will always be fired exactly one time. If no animations are created by the changes in `body`, then the callback will be called immediately after `body`.

## See Also

### Managing animations

var animation: Animation?

The animation, if any, associated with the current state change.

var disablesAnimations: Bool

A Boolean value that indicates whether views should disable animations.


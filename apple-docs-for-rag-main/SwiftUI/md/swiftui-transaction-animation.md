

- SwiftUI
- Transaction
-  animation 

Instance Property

# animation

The animation, if any, associated with the current state change.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var animation: Animation? { get set }
```

## See Also

### Managing animations

var disablesAnimations: Bool

A Boolean value that indicates whether views should disable animations.

func addAnimationCompletion(criteria: AnimationCompletionCriteria, () -> Void)

Adds a completion to run when the animations created with this transaction are all complete.


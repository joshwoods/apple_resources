

- SwiftUI
- TransitionPhase
-  TransitionPhase.didDisappear 

Case

# TransitionPhase.didDisappear

The transition is being applied to a view that has been requested to be removed from the view hierarchy.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case didDisappear
```

## Discussion

In this phase, a transition should show the appearance that will be animated to to make the disappearance transition.

## See Also

### Getting the phase

case identity

The transition is being applied to a view that is in the view hierarchy.

case willAppear

The transition is being applied to a view that is about to be inserted into the view hierarchy.


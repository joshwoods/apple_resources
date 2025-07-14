

- SwiftUI
- ScrollTransitionPhase
-  ScrollTransitionPhase.identity 

Case

# ScrollTransitionPhase.identity

The scroll transition is being applied to a view that is in the visible area.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case identity
```

## Discussion

In this phase, a transition should show its steady state appearance, which will generally not make any visual change to the view.

## See Also

### Getting the phase

case topLeading

The scroll transition is being applied to a view that is about to move into the visible area at the top edge of a vertical scroll view, or the leading edge of a horizont scroll view.

case bottomTrailing

The scroll transition is being applied to a view that is about to move into the visible area at the bottom edge of a vertical scroll view, or the trailing edge of a horizontal scroll view.


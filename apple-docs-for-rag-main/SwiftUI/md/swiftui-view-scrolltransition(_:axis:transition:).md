

- SwiftUI
- View
-  scrollTransition(\_:axis:transition:) 

Instance Method

# scrollTransition(\_:axis:transition:)

Applies the given transition, animating between the phases of the transition as this view appears and disappears within the visible region of the containing scroll view, or other container specified using the `coordinateSpace` parameter.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func scrollTransition(
    _ configuration: ScrollTransitionConfiguration = .interactive,
    axis: Axis? = nil,
    transition: @escaping (EmptyVisualEffect, ScrollTransitionPhase) -> some VisualEffect
) -> some View
```

## Parameters 

`configuration`  

The configuration controlling how the transition will be applied. The configuration will be applied both while the view is coming into view and while it is disappearing (the transition is symmetrical).

`axis`  

The axis of the containing scroll view over which the transition will be applied. The default value of `nil` uses the axis of the innermost containing scroll view, or `.vertical` if the innermost scroll view is scrollable along both axes.

`transition`  

A closure that applies visual effects as a function of the provided phase.

## See Also

### Animating scroll transitions

func scrollTransition(topLeading: ScrollTransitionConfiguration, bottomTrailing: ScrollTransitionConfiguration, axis: Axis?, transition: (EmptyVisualEffect, ScrollTransitionPhase) -> some VisualEffect) -> some View

Applies the given transition, animating between the phases of the transition as this view appears and disappears within the visible region of the containing scroll view, or other container specified using the `coordinateSpace` parameter.

enum ScrollTransitionPhase

The phases that a view transitions between when it scrolls among other views.

struct ScrollTransitionConfiguration

The configuration of a scroll transition that controls how a transition is applied as a view is scrolled through the visible region of a containing scroll view or other container.




- RealityKit
- RealityViewAttachmentBuilderContent
-  scrollTransition(\_:axis:transition:) 

Instance Method

# scrollTransition(\_:axis:transition:)

Applies the given transition, animating between the phases of the transition as this view appears and disappears within the visible region of the containing scroll view, or other container specified using the `coordinateSpace` parameter.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

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

`coordinateSpace`  

The coordinate space of the container that visibility is evaluated within. Defaults to `.scrollView`.

`transition`  

A closure that applies visual effects as a function of the provided phase.


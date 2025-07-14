

- MapKit
- MKAnnotationView
- MKAnnotationView.DragState
-  MKAnnotationView.DragState.none 

Case

# MKAnnotationView.DragState.none

An annotation view that doesn’t have a drag operation.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
case none
```

## Discussion

The view isn’t involved in a drag operation. The annotation view is responsible for returning itself to this state when a drag ends or cancels.

## See Also

### Constants

case starting

An annotation view begins dragging.

case dragging

An annotation view is actively dragging.

case canceling

An annotation view cancels drag operation.

case ending

An annotation view ends dragging.


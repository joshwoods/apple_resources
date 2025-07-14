

- MapKit
- MKAnnotationView
- MKAnnotationView.DragState
-  MKAnnotationView.DragState.canceling 

Case

# MKAnnotationView.DragState.canceling

An annotation view cancels drag operation.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
case canceling
```

## Discussion

A user action causes the view to cancel the drag operation. You can put an annotation view into this state to abort the operation.

## See Also

### Constants

case none

An annotation view that doesn’t have a drag operation.

case starting

An annotation view begins dragging.

case dragging

An annotation view is actively dragging.

case ending

An annotation view ends dragging.


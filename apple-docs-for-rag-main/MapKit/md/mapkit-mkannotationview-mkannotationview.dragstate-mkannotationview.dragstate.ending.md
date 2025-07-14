

- MapKit
- MKAnnotationView
- MKAnnotationView.DragState
-  MKAnnotationView.DragState.ending 

Case

# MKAnnotationView.DragState.ending

An annotation view ends dragging.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
case ending
```

## Discussion

A user action indicates the user dropped the view. The map view automatically moves annotation views to this state in response to appropriate user actions.

## See Also

### Constants

case none

An annotation view that doesn’t have a drag operation.

case starting

An annotation view begins dragging.

case dragging

An annotation view is actively dragging.

case canceling

An annotation view cancels drag operation.




- MapKit
- MKAnnotationView
-  dragState 

Instance Property

# dragState

The drag state of the annotation view.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
@MainActor
var dragState: MKAnnotationView.DragState { get set }
```

## Discussion

If your app runs in iOS 4.2 or later, override the setDragState(_:animated:) method and use it to manage the drag state instead.

To support drag operations, override the implementation of this property and update the drag state at the following times:

- When the drag state changes to MKAnnotationView.DragState.starting, set the state to MKAnnotationView.DragState.dragging. If you perform an animation to indicate the beginning of a drag, perform that animation before changing the state. Changing the state to the new value lets the map know when your animations complete.

- When the state changes to either MKAnnotationView.DragState.canceling or MKAnnotationView.DragState.ending, set the state to MKAnnotationView.DragState.none. If you perform an animation at the end of a drag, perform that animation before changing the state.

Changing the state to the MKAnnotationView.DragState.dragging or MKAnnotationView.DragState.none value is the way to signal to the map view when you finish performing animations. For example, when a drag operation begins for an annotation, the class executes an animation to lift the view off the map. Similarly, when the user drops the annotation, the class performs a drop animation. Even if you don’t perform any animations, it’s best practice to change the value of this property to reflect the correct state.

Don’t try to stop a new drag operation by changing the state from `starting` to `none`. If you don’t want your annotation view to be draggable, set the isDraggable property to false.

## See Also

### Supporting drag operations

var isDraggable: Bool

A Boolean value that indicates whether the annotation view is draggable.

func setDragState(MKAnnotationView.DragState, animated: Bool)

Sets the drag state for the annotation view.


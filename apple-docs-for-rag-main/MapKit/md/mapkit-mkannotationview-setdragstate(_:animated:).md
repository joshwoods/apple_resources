

- MapKit
- MKAnnotationView
-  setDragState(\_:animated:) 

Instance Method

# setDragState(\_:animated:)

Sets the drag state for the annotation view.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
@MainActor
func setDragState(
    _ newDragState: MKAnnotationView.DragState,
    animated: Bool
)
```

## Parameters 

`newDragState`  

The new drag state for the annotation view.

`animated`  

If true, the map view animates the change to the new drag state; otherwise, the map view makes the change without animations.

## Discussion

Apps can override this method and use it to implement drag support for custom annotation views. As the system detects user actions that indicate a drag, it calls this method to update the drag state. In response to these changes, your custom implementation of this method needs to do the following:

- When the drag state changes to MKAnnotationView.DragState.starting, set the state to MKAnnotationView.DragState.dragging. If you perform an animation to indicate the beginning of a drag, and the `animated` parameter is true, perform that animation before changing the state.

- When the state changes to either MKAnnotationView.DragState.canceling or MKAnnotationView.DragState.ending, set the state to MKAnnotationView.DragState.none. If you perform an animation at the end of a drag, and the `animated` parameter is true, perform that animation before changing the state.

The default implementation of this method sets the value of the dragState property to the value in the `newDragState` parameter only. Therefore, direct subclasses can call the inherited version of this method to change the drag state; otherwise, change the value in the isDraggable property directly.

Changing the state to MKAnnotationView.DragState.dragging or MKAnnotationView.DragState.none is the way to signal to the map view when you finish performing animations. For example, when a drag operation begins for an annotation, the class executes an animation to lift the view off the map. Similarly, when the user drops the annotation, the class performs a drop animation. Even if you don’t perform any animations, call the inherited version of this method to update the dragState property.

Don’t try to stop a new drag operation by changing the state from MKAnnotationView.DragState.starting to MKAnnotationView.DragState.none. If you don’t want your annotation view to be draggable, set the isDraggable property to false.

## See Also

### Supporting drag operations

var isDraggable: Bool

A Boolean value that indicates whether the annotation view is draggable.

var dragState: MKAnnotationView.DragState

The drag state of the annotation view.


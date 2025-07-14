

- MapKit
- MKAnnotationView
-  isDraggable 

Instance Property

# isDraggable

A Boolean value that indicates whether the annotation view is draggable.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
@MainActor
var isDraggable: Bool { get set }
```

## Discussion

Setting this property to true makes an annotation draggable by the user. If true, the associated annotation object needs to also implement the setCoordinate: method. The default value of this property is false.

Setting this property to true lets the map view know that the annotation is draggable. You can’t conditionalize drag operations by attempting to stop an operation the user initiates. Doing so can lead to undefined behavior. After it begins, the drag operation needs to continue to completion.

## See Also

### Supporting drag operations

func setDragState(MKAnnotationView.DragState, animated: Bool)

Sets the drag state for the annotation view.

var dragState: MKAnnotationView.DragState

The drag state of the annotation view.


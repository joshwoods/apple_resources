

- AppKit
- NSDraggingInfo
-  animatesToDestination 

Instance Property

# animatesToDestination

A Boolean value that indicates whether the dragging formation animates while the drag is over the destination.

macOS 10.7+

``` source
@MainActor
var animatesToDestination: Bool { get set }
```

**Required**

## Discussion

During the conclusion of an accepted drag, if this property is set to true, the drag manager will animate each dragging image to their NSDraggingFormation.none locations. Otherwise, the drag images are removed without any animation.

This property is inspected between prepareForDragOperation: and performDragOperation:. You should enumerate through the dragging items during performDragOperation: to set the item’s draggingFrame to the correct destinations.

## See Also

### Sliding the image

func slideDraggedImage(to: NSPoint)

Slides the image to a specified location.

**Required**

var draggingFormation: NSDraggingFormation

The formation of the dragging items while the drag is over the destination.

**Required**


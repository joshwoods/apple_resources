

- AppKit
- NSDraggingInfo
-  slideDraggedImage(to:) 

Instance Method

# slideDraggedImage(to:)

Slides the image to a specified location.

macOS

``` source
@MainActor
func slideDraggedImage(to screenPoint: NSPoint)
```

**Required**

## Parameters 

`screenPoint`  

A point that specifies a location in the screen coordinate system.

## Discussion

This method can be used to adjust the location to which the dragged image will slide back if the drag is rejected.

It should only be invoked from within the destination’s implementation of prepareForDragOperation:, and will only have effect if the destination rejects the drag.

This method is invoked after the user has released the image but before it is removed from the screen.

### Special Considerations

This method has been available since OS X v 10.0, however it was not implemented until OS X v 10.5. Previous to that version, it did nothing.

## See Also

### Sliding the image

var animatesToDestination: Bool

A Boolean value that indicates whether the dragging formation animates while the drag is over the destination.

**Required**

var draggingFormation: NSDraggingFormation

The formation of the dragging items while the drag is over the destination.

**Required**


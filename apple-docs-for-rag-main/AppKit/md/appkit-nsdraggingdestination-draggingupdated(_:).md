

- AppKit
- NSDraggingDestination
-  draggingUpdated(\_:) 

Instance Method

# draggingUpdated(\_:)

Invoked periodically as the image is held within the destination area, allowing modification of the dragging operation or mouse-pointer position.

macOS

``` source
@MainActor
optional func draggingUpdated(_ sender: any NSDraggingInfo) -> NSDragOperation
```

## Parameters 

`sender`  

The object sending the message; use it to get details about the dragging operation.

## Return Value

One (and only one) of the dragging operation constants described in NSDragOperation in the NSDraggingInfo reference. The default return value (if this method is not implemented by the destination) is the value returned by the previous draggingEntered(_:) message.

## Discussion

For this to be invoked, the destination must have registered for the pasteboard data type involved in the drag operation. The messages continue until the image is either released or dragged out of the window or view.

This method provides the destination with an opportunity to modify the dragging operation depending on the position of the mouse pointer inside of the destination view or window object. For example, you may have several graphics or areas of text contained within the same view and wish to tailor the dragging operation, or to ignore the drag event completely, depending upon which object is underneath the mouse pointer at the time when the user releases the dragged image and the performDragOperation(_:) method is invoked.

You typically examine the contents of the pasteboard in the draggingEntered(_:) method, where this examination is performed only once, rather than in the draggingUpdated(_:) method, which is invoked multiple times.

Only one destination at a time receives a sequence of draggingUpdated(_:) messages. If the mouse pointer is within the bounds of two overlapping views that are both valid destinations, the uppermost view receives these messages until the image is either released or dragged out.

## See Also

### Related Documentation

func prepareForDragOperation(any NSDraggingInfo) -> Bool

Invoked when the image is released, allowing the receiver to agree to or refuse drag operation.

### Managing a Dragging Session Before an Image Is Released

func draggingEntered(any NSDraggingInfo) -> NSDragOperation

Invoked when the dragged image enters destination bounds or frame; delegate returns dragging operation to perform.

func wantsPeriodicDraggingUpdates() -> Bool

Asks the destination object whether it wants to receive periodic draggingUpdated(_:) messages.

func draggingExited((any NSDraggingInfo)?)

Invoked when the dragged image exits the destination’s bounds rectangle (in the case of a view object) or its frame rectangle (in the case of a window object).

func draggingEnded(any NSDraggingInfo)

Called when a drag operation ends.


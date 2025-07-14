

- AppKit
- NSDraggingDestination
-  draggingEntered(\_:) 

Instance Method

# draggingEntered(\_:)

Invoked when the dragged image enters destination bounds or frame; delegate returns dragging operation to perform.

macOS

``` source
@MainActor
optional func draggingEntered(_ sender: any NSDraggingInfo) -> NSDragOperation
```

## Parameters 

`sender`  

The object sending the message; use it to get details about the dragging operation.

## Return Value

One (and only one) of the dragging operation constants described in NSDragOperation in the NSDraggingInfo reference. The default return value (if this method is not implemented by the destination) is the value returned by the previous draggingEntered(_:) message.

## Discussion

Invoked when a dragged image enters the destination but only if the destination has registered for the pasteboard data type involved in the drag operation. Specifically, this method is invoked when the mouse pointer enters the destination’s bounds rectangle (if it is a view object) or its frame rectangle (if it is a window object).

This method must return a value that indicates which dragging operation the destination will perform when the image is released. In deciding which dragging operation to return, the method should evaluate the overlap between both the dragging operations allowed by the source (obtained from `sender` with the draggingSourceOperationMask method) and the dragging operations and pasteboard data types the destination itself supports.

If none of the operations is appropriate, this method should return `NSDragOperationNone` (this is the default response if the method is not implemented by the destination). A destination will still receive draggingUpdated(_:) and draggingExited(_:) even if `NSDragOperationNone` is returned by this method.

## See Also

### Related Documentation

Drag and Drop Programming Topics

func prepareForDragOperation(any NSDraggingInfo) -> Bool

Invoked when the image is released, allowing the receiver to agree to or refuse drag operation.

### Managing a Dragging Session Before an Image Is Released

func wantsPeriodicDraggingUpdates() -> Bool

Asks the destination object whether it wants to receive periodic draggingUpdated(_:) messages.

func draggingUpdated(any NSDraggingInfo) -> NSDragOperation

Invoked periodically as the image is held within the destination area, allowing modification of the dragging operation or mouse-pointer position.

func draggingExited((any NSDraggingInfo)?)

Invoked when the dragged image exits the destination’s bounds rectangle (in the case of a view object) or its frame rectangle (in the case of a window object).

func draggingEnded(any NSDraggingInfo)

Called when a drag operation ends.


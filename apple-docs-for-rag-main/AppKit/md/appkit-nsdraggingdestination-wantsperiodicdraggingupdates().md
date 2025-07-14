

- AppKit
- NSDraggingDestination
-  wantsPeriodicDraggingUpdates() 

Instance Method

# wantsPeriodicDraggingUpdates()

Asks the destination object whether it wants to receive periodic draggingUpdated(_:) messages.

macOS

``` source
@MainActor
optional func wantsPeriodicDraggingUpdates() -> Bool
```

## Return Value

true if the destination wants to receive periodic draggingUpdated(_:) messages, false otherwise.

## Discussion

If the destination returns false, these messages are sent only when the mouse moves or a modifier flag changes. Otherwise the destination gets the default behavior, where it receives periodic dragging-updated messages even if nothing changes.

## See Also

### Managing a Dragging Session Before an Image Is Released

func draggingEntered(any NSDraggingInfo) -> NSDragOperation

Invoked when the dragged image enters destination bounds or frame; delegate returns dragging operation to perform.

func draggingUpdated(any NSDraggingInfo) -> NSDragOperation

Invoked periodically as the image is held within the destination area, allowing modification of the dragging operation or mouse-pointer position.

func draggingExited((any NSDraggingInfo)?)

Invoked when the dragged image exits the destination’s bounds rectangle (in the case of a view object) or its frame rectangle (in the case of a window object).

func draggingEnded(any NSDraggingInfo)

Called when a drag operation ends.


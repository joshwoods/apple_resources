

- AppKit
- NSDraggingDestination
-  draggingExited(\_:) 

Instance Method

# draggingExited(\_:)

Invoked when the dragged image exits the destination’s bounds rectangle (in the case of a view object) or its frame rectangle (in the case of a window object).

macOS

``` source
@MainActor
optional func draggingExited(_ sender: (any NSDraggingInfo)?)
```

## Parameters 

`sender`  

The object sending the message; use it to get details about the dragging operation.

## See Also

### Managing a Dragging Session Before an Image Is Released

func draggingEntered(any NSDraggingInfo) -> NSDragOperation

Invoked when the dragged image enters destination bounds or frame; delegate returns dragging operation to perform.

func wantsPeriodicDraggingUpdates() -> Bool

Asks the destination object whether it wants to receive periodic draggingUpdated(_:) messages.

func draggingUpdated(any NSDraggingInfo) -> NSDragOperation

Invoked periodically as the image is held within the destination area, allowing modification of the dragging operation or mouse-pointer position.

func draggingEnded(any NSDraggingInfo)

Called when a drag operation ends.




- AppKit
- NSDraggingDestination
-  draggingEnded(\_:) 

Instance Method

# draggingEnded(\_:)

Called when a drag operation ends.

macOS

``` source
@MainActor
optional func draggingEnded(_ sender: any NSDraggingInfo)
```

## Parameters 

`sender`  

The object sending the message; use it to get details about the dragging operation.

## Discussion

Implement this method if you want to be notified when a drag operation ends, which can be useful if the drag ends in some other destination. For example, this method might be used by a destination doing auto-expansion in order to collapse any auto-expands.

## See Also

### Managing a Dragging Session Before an Image Is Released

func draggingEntered(any NSDraggingInfo) -> NSDragOperation

Invoked when the dragged image enters destination bounds or frame; delegate returns dragging operation to perform.

func wantsPeriodicDraggingUpdates() -> Bool

Asks the destination object whether it wants to receive periodic draggingUpdated(_:) messages.

func draggingUpdated(any NSDraggingInfo) -> NSDragOperation

Invoked periodically as the image is held within the destination area, allowing modification of the dragging operation or mouse-pointer position.

func draggingExited((any NSDraggingInfo)?)

Invoked when the dragged image exits the destination’s bounds rectangle (in the case of a view object) or its frame rectangle (in the case of a window object).


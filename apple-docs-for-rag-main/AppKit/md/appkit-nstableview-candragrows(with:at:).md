

- AppKit
- NSTableView
-  canDragRows(with:at:) 

Instance Method

# canDragRows(with:at:)

Returns a Boolean value indicating whether the table view allows dragging the rows with the drag initiated at the specified point.

macOS

``` source
@MainActor
func canDragRows(
    with rowIndexes: IndexSet,
    at mouseDownPoint: NSPoint
) -> Bool
```

## Parameters 

`rowIndexes`  

The row indexes to drag.

`mouseDownPoint`  

The location where the drag was initiated.

## Return Value

false to disallow the drag.

## See Also

### Dragging

func dragImageForRows(with: IndexSet, tableColumns: [NSTableColumn], event: NSEvent, offset: NSPointPointer) -> NSImage

Computes and returns an image to use for dragging.

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Sets the default operation mask returned by `draggingSourceOperationMaskForLocal:` to `mask`.

var verticalMotionCanBeginDrag: Bool

A Boolean value indicating whether vertical motion is treated as a drag or selection change.

var draggingDestinationFeedbackStyle: NSTableView.DraggingDestinationFeedbackStyle

The feedback style displayed when the user drags over the table view.

func setDropRow(Int, dropOperation: NSTableView.DropOperation)

Retargets the proposed drop operation.


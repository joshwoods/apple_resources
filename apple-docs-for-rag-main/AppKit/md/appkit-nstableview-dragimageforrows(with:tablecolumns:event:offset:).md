

- AppKit
- NSTableView
-  dragImageForRows(with:tableColumns:event:offset:) 

Instance Method

# dragImageForRows(with:tableColumns:event:offset:)

Computes and returns an image to use for dragging.

macOS

``` source
@MainActor
func dragImageForRows(
    with dragRows: IndexSet,
    tableColumns: [NSTableColumn],
    event dragEvent: NSEvent,
    offset dragImageOffset: NSPointPointer
) -> NSImage
```

## Parameters 

`dragRows`  

An index set containing the row indexes that should be in the image.

`tableColumns`  

An array of table columns that should be in the image.

`dragEvent`  

The event that initiated the drag.

`dragImageOffset`  

An in/out parameter specifying the offset of the cursor in the image, the default value is NSZeroPoint. Returning NSZeroPoint causes the cursor to be centered.

## Return Value

An `NSImage` containing a custom image for the specified rows and columns participating in the drag.

## See Also

### Dragging

func canDragRows(with: IndexSet, at: NSPoint) -> Bool

Returns a Boolean value indicating whether the table view allows dragging the rows with the drag initiated at the specified point.

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Sets the default operation mask returned by `draggingSourceOperationMaskForLocal:` to `mask`.

var verticalMotionCanBeginDrag: Bool

A Boolean value indicating whether vertical motion is treated as a drag or selection change.

var draggingDestinationFeedbackStyle: NSTableView.DraggingDestinationFeedbackStyle

The feedback style displayed when the user drags over the table view.

func setDropRow(Int, dropOperation: NSTableView.DropOperation)

Retargets the proposed drop operation.


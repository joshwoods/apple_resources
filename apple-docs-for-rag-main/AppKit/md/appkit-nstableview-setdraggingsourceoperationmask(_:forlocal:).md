

- AppKit
- NSTableView
-  setDraggingSourceOperationMask(\_:forLocal:) 

Instance Method

# setDraggingSourceOperationMask(\_:forLocal:)

Sets the default operation mask returned by `draggingSourceOperationMaskForLocal:` to `mask`.

macOS

``` source
@MainActor
func setDraggingSourceOperationMask(
    _ mask: NSDragOperation,
    forLocal isLocal: Bool
)
```

## Parameters 

`mask`  

The drag operation mask. See NSDragOperation for the supported values.

`isLocal`  

true if the destination is the same application, otherwise false. In either case the specified `mask` value is archived and used.

## See Also

### Dragging

func dragImageForRows(with: IndexSet, tableColumns: [NSTableColumn], event: NSEvent, offset: NSPointPointer) -> NSImage

Computes and returns an image to use for dragging.

func canDragRows(with: IndexSet, at: NSPoint) -> Bool

Returns a Boolean value indicating whether the table view allows dragging the rows with the drag initiated at the specified point.

var verticalMotionCanBeginDrag: Bool

A Boolean value indicating whether vertical motion is treated as a drag or selection change.

var draggingDestinationFeedbackStyle: NSTableView.DraggingDestinationFeedbackStyle

The feedback style displayed when the user drags over the table view.

func setDropRow(Int, dropOperation: NSTableView.DropOperation)

Retargets the proposed drop operation.




- AppKit
- NSTableView
-  verticalMotionCanBeginDrag 

Instance Property

# verticalMotionCanBeginDrag

A Boolean value indicating whether vertical motion is treated as a drag or selection change.

macOS

``` source
@MainActor
var verticalMotionCanBeginDrag: Bool { get set }
```

## Discussion

The default value of this property is true, which indicates that a vertical drag motion begins a drag. In this case a vertical drag will drag-select rows. Most often, you would want to disable vertical dragging when it’s expected that horizontal dragging is the natural motion.

Note

Horizontal motion is always a valid motion to begin a drag.

## See Also

### Dragging

func dragImageForRows(with: IndexSet, tableColumns: [NSTableColumn], event: NSEvent, offset: NSPointPointer) -> NSImage

Computes and returns an image to use for dragging.

func canDragRows(with: IndexSet, at: NSPoint) -> Bool

Returns a Boolean value indicating whether the table view allows dragging the rows with the drag initiated at the specified point.

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Sets the default operation mask returned by `draggingSourceOperationMaskForLocal:` to `mask`.

var draggingDestinationFeedbackStyle: NSTableView.DraggingDestinationFeedbackStyle

The feedback style displayed when the user drags over the table view.

func setDropRow(Int, dropOperation: NSTableView.DropOperation)

Retargets the proposed drop operation.




- AppKit
- NSTableView
-  draggingDestinationFeedbackStyle 

Instance Property

# draggingDestinationFeedbackStyle

The feedback style displayed when the user drags over the table view.

macOS 10.6+

``` source
@MainActor
var draggingDestinationFeedbackStyle: NSTableView.DraggingDestinationFeedbackStyle { get set }
```

## Discussion

The default value of this property is NSTableView.DraggingDestinationFeedbackStyle.regular. However, changing the selection highlight style to NSTableView.SelectionHighlightStyle.sourceList automatically changes the value of this property to NSTableView.DraggingDestinationFeedbackStyle.sourceList.

## See Also

### Dragging

func dragImageForRows(with: IndexSet, tableColumns: [NSTableColumn], event: NSEvent, offset: NSPointPointer) -> NSImage

Computes and returns an image to use for dragging.

func canDragRows(with: IndexSet, at: NSPoint) -> Bool

Returns a Boolean value indicating whether the table view allows dragging the rows with the drag initiated at the specified point.

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Sets the default operation mask returned by `draggingSourceOperationMaskForLocal:` to `mask`.

var verticalMotionCanBeginDrag: Bool

A Boolean value indicating whether vertical motion is treated as a drag or selection change.

func setDropRow(Int, dropOperation: NSTableView.DropOperation)

Retargets the proposed drop operation.


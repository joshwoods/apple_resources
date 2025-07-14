

- AppKit
- NSBrowser
-  canDragRows(with:inColumn:with:) 

Instance Method

# canDragRows(with:inColumn:with:)

Indicates whether the browser can attempt to initiate a drag of the given rows for the given event.

macOS 10.5+

``` source
@MainActor
func canDragRows(
    with rowIndexes: IndexSet,
    inColumn column: Int,
    with event: NSEvent
) -> Bool
```

## Parameters 

`rowIndexes`  

Rows the user is dragging

`column`  

Column containing the rows the user is dragging.

`event`  

Mouse-drag event.

## Return Value

true when `rowIndexes` identifies at least one row and all the identified rows are enabled; otherwise, false.

## See Also

### Related Documentation

func browser(NSBrowser, canDragRowsWith: IndexSet, inColumn: Int, with: NSEvent) -> Bool

Sent to the delegate to determine whether the browser can attempt to initiate a drag of the specified rows for the specified event.

### Dragging

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Specifies the drag-operation mask for dragging operations with local or external destinations.

func draggingImageForRows(with: IndexSet, inColumn: Int, with: NSEvent, offset: NSPointPointer?) -> NSImage?

Provides an image to represent dragged rows during a drag operation on the browser.




- AppKit
- NSBrowser
-  draggingImageForRows(with:inColumn:with:offset:) 

Instance Method

# draggingImageForRows(with:inColumn:with:offset:)

Provides an image to represent dragged rows during a drag operation on the browser.

macOS 10.5+

``` source
@MainActor
func draggingImageForRows(
    with rowIndexes: IndexSet,
    inColumn column: Int,
    with event: NSEvent,
    offset dragImageOffset: NSPointPointer?
) -> NSImage?
```

## Parameters 

`rowIndexes`  

Rows the user is dragging.

`column`  

Column with the rows the user is dragging.

`event`  

Mouse drag event.

`dragImageOffset`  

Offset for the returned image:

- NSZeroPoint: The image is centered under the pointer.

## Return Value

Image representing the visible cells identified by rowIndexes.

## See Also

### Related Documentation

func browser(NSBrowser, draggingImageForRowsWith: IndexSet, inColumn: Int, with: NSEvent, offset: NSPointPointer) -> NSImage?

Sent to the delegate to obtain an image to represent dragged rows during a drag operation on a browser.

### Dragging

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Specifies the drag-operation mask for dragging operations with local or external destinations.

func canDragRows(with: IndexSet, inColumn: Int, with: NSEvent) -> Bool

Indicates whether the browser can attempt to initiate a drag of the given rows for the given event.


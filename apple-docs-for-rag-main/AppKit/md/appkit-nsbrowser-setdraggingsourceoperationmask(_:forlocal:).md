

- AppKit
- NSBrowser
-  setDraggingSourceOperationMask(\_:forLocal:) 

Instance Method

# setDraggingSourceOperationMask(\_:forLocal:)

Specifies the drag-operation mask for dragging operations with local or external destinations.

macOS 10.5+

``` source
@MainActor
func setDraggingSourceOperationMask(
    _ mask: NSDragOperation,
    forLocal isLocal: Bool
)
```

## Parameters 

`mask`  

Dragging operation mask to use for either local or external drag operations, as specified by localDestination.

`isLocal`  

Indicates the location of the dragging operation’s destination object:

true for this application; false for another application.

## Discussion

Important

Do not override this method.

## See Also

### Dragging

func canDragRows(with: IndexSet, inColumn: Int, with: NSEvent) -> Bool

Indicates whether the browser can attempt to initiate a drag of the given rows for the given event.

func draggingImageForRows(with: IndexSet, inColumn: Int, with: NSEvent, offset: NSPointPointer?) -> NSImage?

Provides an image to represent dragged rows during a drag operation on the browser.


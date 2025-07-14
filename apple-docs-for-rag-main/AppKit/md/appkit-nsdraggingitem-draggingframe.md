

- AppKit
- NSDraggingItem
-  draggingFrame 

Instance Property

# draggingFrame

The frame of the dragging item.

macOS 10.7+

``` source
var draggingFrame: NSRect { get set }
```

## Discussion

The dragging frame provides the spatial relationship between NSDraggingItem instances when you set the dragging formation to NSDraggingFormation.none.

The exact coordinate space of this rectangle depends on where you use it. Examples are the view that initiates the drag using beginDraggingSession(with:event:source:) or the view you pass to the NSDraggingSession implementation of enumerateDraggingItems(options:for:classes:searchOptions:using:).

## See Also

### Dragging frame

func setDraggingFrame(NSRect, contents: Any?)

Sets the item’s dragging frame and contents.


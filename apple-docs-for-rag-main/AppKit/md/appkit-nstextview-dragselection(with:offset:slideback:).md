

- AppKit
- NSTextView
-  dragSelection(with:offset:slideBack:) 

Instance Method

# dragSelection(with:offset:slideBack:)

Begins dragging the current selected text range.

macOS

``` source
@MainActor
func dragSelection(
    with event: NSEvent,
    offset mouseOffset: NSSize,
    slideBack: Bool
) -> Bool
```

## Parameters 

`event`  

The event that initiated dragging the selection.

`mouseOffset`  

The cursor’s current location relative to the mouse-down `event`.

`slideBack`  

true if the image being dragged should slide back to its original position if the drag does not succeed, false otherwise.

## Return Value

true if the drag can be successfully initiated, false otherwise.

## Discussion

Primarily for subclasses, who can override it to intervene at the beginning of a drag.

## See Also

### Dragging

func dragImageForSelection(with: NSEvent, origin: NSPointPointer?) -> NSImage?

Returns an appropriate drag image for the drag initiated by the specified event.

func dragOperation(for: any NSDraggingInfo, type: NSPasteboard.PasteboardType) -> NSDragOperation

Returns the type of drag operation that should be performed if the image were released now.

var acceptsGlyphInfo: Bool

A Boolean value that indicates whether the receiver accepts the glyph info attribute.




- AppKit
- NSTextView
-  dragImageForSelection(with:origin:) 

Instance Method

# dragImageForSelection(with:origin:)

Returns an appropriate drag image for the drag initiated by the specified event.

macOS

``` source
@MainActor
func dragImageForSelection(
    with event: NSEvent,
    origin: NSPointPointer?
) -> NSImage?
```

## Parameters 

`event`  

The event that initiated the drag session.

`origin`  

On return, the lower-left point of the image in view coordinates.

## Return Value

An appropriate drag image for the drag initiated by `event`. May be `nil`, in which case a default icon will be used.

## Discussion

This method is used by dragSelection(with:offset:slideBack:). It can be called by others who need such an image, or can be overridden by subclasses to return a different image.

## See Also

### Dragging

func dragOperation(for: any NSDraggingInfo, type: NSPasteboard.PasteboardType) -> NSDragOperation

Returns the type of drag operation that should be performed if the image were released now.

func dragSelection(with: NSEvent, offset: NSSize, slideBack: Bool) -> Bool

Begins dragging the current selected text range.

var acceptsGlyphInfo: Bool

A Boolean value that indicates whether the receiver accepts the glyph info attribute.


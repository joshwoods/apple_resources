

- AppKit
- NSTextView
-  acceptsGlyphInfo 

Instance Property

# acceptsGlyphInfo

A Boolean value that indicates whether the receiver accepts the glyph info attribute.

macOS

``` source
@MainActor
var acceptsGlyphInfo: Bool { get set }
```

## Discussion

true if the receiver accepts the `NSGlyphInfoAttributeName` attribute from text input sources such as input methods and the pasteboard, false otherwise.

## See Also

### Dragging

func dragImageForSelection(with: NSEvent, origin: NSPointPointer?) -> NSImage?

Returns an appropriate drag image for the drag initiated by the specified event.

func dragOperation(for: any NSDraggingInfo, type: NSPasteboard.PasteboardType) -> NSDragOperation

Returns the type of drag operation that should be performed if the image were released now.

func dragSelection(with: NSEvent, offset: NSSize, slideBack: Bool) -> Bool

Begins dragging the current selected text range.


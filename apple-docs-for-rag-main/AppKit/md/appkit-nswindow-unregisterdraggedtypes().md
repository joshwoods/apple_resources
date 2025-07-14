

- AppKit
- NSWindow
-  unregisterDraggedTypes() 

Instance Method

# unregisterDraggedTypes()

Unregisters the window as a possible destination for dragging operations.

macOS

``` source
@MainActor
func unregisterDraggedTypes()
```

## See Also

### Dragging Items

func drag(NSImage, at: NSPoint, offset: NSSize, event: NSEvent, pasteboard: NSPasteboard, source: Any, slideBack: Bool)

Begins a dragging session.

Deprecated

func registerForDraggedTypes([NSPasteboard.PasteboardType])

Registers a set of pasteboard types that the window accepts as the destination of an image-dragging session.


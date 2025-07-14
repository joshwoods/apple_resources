

- AppKit
- NSWindow
-  registerForDraggedTypes(\_:) 

Instance Method

# registerForDraggedTypes(\_:)

Registers a set of pasteboard types that the window accepts as the destination of an image-dragging session.

macOS

``` source
@MainActor
func registerForDraggedTypes(_ newTypes: [NSPasteboard.PasteboardType])
```

## Parameters 

`newTypes`  

An array of the pasteboard types the window accepts as the destination of an image-dragging session.

## Discussion

Registering an `NSWindow` object for dragged types automatically makes it a candidate destination object for a dragging session. `NSWindow` has a default implementation for many of the methods in the NSDraggingDestination protocol. The default implementation forwards each message to the delegate if the delegate responds to the selector of the message. The messages forwarded this way are draggingEntered(_:), draggingUpdated(_:), draggingExited(_:), prepareForDragOperation(_:), performDragOperation(_:), and concludeDragOperation(_:).

## See Also

### Dragging Items

func drag(NSImage, at: NSPoint, offset: NSSize, event: NSEvent, pasteboard: NSPasteboard, source: Any, slideBack: Bool)

Begins a dragging session.

Deprecated

func unregisterDraggedTypes()

Unregisters the window as a possible destination for dragging operations.


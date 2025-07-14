

- AppKit
- NSView
-  unregisterDraggedTypes() 

Instance Method

# unregisterDraggedTypes()

Unregisters the view as a possible destination in a dragging session.

macOS

``` source
@MainActor
func unregisterDraggedTypes()
```

## See Also

### Dragging Operations

func registerForDraggedTypes([NSPasteboard.PasteboardType])

Registers the pasteboard types that the view will accept as the destination of an image-dragging session.

var registeredDraggedTypes: [NSPasteboard.PasteboardType]

The array of pasteboard drag types that the view can accept.

func beginDraggingSession(with: [NSDraggingItem], event: NSEvent, source: any NSDraggingSource) -> NSDraggingSession

Initiates a dragging session with a group of dragging items.

func shouldDelayWindowOrdering(for: NSEvent) -> Bool

Allows the user to drag objects from the view without activating the app or moving the window of the view forward, possibly obscuring the destination.


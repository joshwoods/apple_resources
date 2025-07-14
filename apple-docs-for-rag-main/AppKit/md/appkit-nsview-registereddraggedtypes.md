

- AppKit
- NSView
-  registeredDraggedTypes 

Instance Property

# registeredDraggedTypes

The array of pasteboard drag types that the view can accept.

macOS

``` source
@MainActor
var registeredDraggedTypes: [NSPasteboard.PasteboardType] { get }
```

## Discussion

This property contains an array of NSString objects, each of which corresponds to a Uniform Type Identifier. The array elements are in no particular order, but the array is guaranteed not to contain duplicate entries. To register your view’s drag types, use the registerForDraggedTypes(_:) method.

## See Also

### Dragging Operations

func registerForDraggedTypes([NSPasteboard.PasteboardType])

Registers the pasteboard types that the view will accept as the destination of an image-dragging session.

func unregisterDraggedTypes()

Unregisters the view as a possible destination in a dragging session.

func beginDraggingSession(with: [NSDraggingItem], event: NSEvent, source: any NSDraggingSource) -> NSDraggingSession

Initiates a dragging session with a group of dragging items.

func shouldDelayWindowOrdering(for: NSEvent) -> Bool

Allows the user to drag objects from the view without activating the app or moving the window of the view forward, possibly obscuring the destination.




- AppKit
- NSView
-  registerForDraggedTypes(\_:) 

Instance Method

# registerForDraggedTypes(\_:)

Registers the pasteboard types that the view will accept as the destination of an image-dragging session.

macOS

``` source
@MainActor
func registerForDraggedTypes(_ newTypes: [NSPasteboard.PasteboardType])
```

## Parameters 

`newTypes`  

An array of Uniform Type Identifier. See System-Declared Uniform Type Identifiers for descriptions of the pasteboard type identifiers.

## Discussion

Registering an `NSView` object for dragged types automatically makes it a candidate destination object for a dragging session. As such, it must properly implement some or all of the `NSDraggingDestination` protocol methods. As a convenience, `NSView` provides default implementations of these methods. See the NSDraggingDestination protocol specification for details.

## See Also

### Dragging Operations

func unregisterDraggedTypes()

Unregisters the view as a possible destination in a dragging session.

var registeredDraggedTypes: [NSPasteboard.PasteboardType]

The array of pasteboard drag types that the view can accept.

func beginDraggingSession(with: [NSDraggingItem], event: NSEvent, source: any NSDraggingSource) -> NSDraggingSession

Initiates a dragging session with a group of dragging items.

func shouldDelayWindowOrdering(for: NSEvent) -> Bool

Allows the user to drag objects from the view without activating the app or moving the window of the view forward, possibly obscuring the destination.


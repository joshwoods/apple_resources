

- AppKit
- NSView
-  shouldDelayWindowOrdering(for:) 

Instance Method

# shouldDelayWindowOrdering(for:)

Allows the user to drag objects from the view without activating the app or moving the window of the view forward, possibly obscuring the destination.

macOS

``` source
@MainActor
func shouldDelayWindowOrdering(for event: NSEvent) -> Bool
```

## Parameters 

`event`  

An object representing an initial mouse-down event.

## Return Value

If this method returns true, the normal window-ordering and activation mechanism is delayed (not necessarily prevented) until the next mouse-up event. If it returns false, then normal ordering and activation occur.

## Discussion

Never invoke this method directly; it’s invoked automatically for each mouse-down event directed at the NSView.

An `NSView` subclass that allows dragging should implement this method to return true if `theEvent` is potentially the beginning of a dragging session or of some other context where window ordering isn’t appropriate. This method is invoked before a mouseDown(with:) message for `theEvent` is sent. The default implementation returns false.

If, after delaying window ordering, the view actually initiates a dragging session or similar operation, it should also send a preventWindowOrdering() message to `NSApp`, which completely prevents the window from ordering forward and the activation from becoming active. preventWindowOrdering() is sent automatically by the `dragImage:` and `dragFile:` methods of `NSView`.

## See Also

### Dragging Operations

func registerForDraggedTypes([NSPasteboard.PasteboardType])

Registers the pasteboard types that the view will accept as the destination of an image-dragging session.

func unregisterDraggedTypes()

Unregisters the view as a possible destination in a dragging session.

var registeredDraggedTypes: [NSPasteboard.PasteboardType]

The array of pasteboard drag types that the view can accept.

func beginDraggingSession(with: [NSDraggingItem], event: NSEvent, source: any NSDraggingSource) -> NSDraggingSession

Initiates a dragging session with a group of dragging items.




- AppKit
- NSView
-  beginDraggingSession(with:event:source:) 

Instance Method

# beginDraggingSession(with:event:source:)

Initiates a dragging session with a group of dragging items.

macOS 10.7+

``` source
@MainActor
func beginDraggingSession(
    with items: [NSDraggingItem],
    event: NSEvent,
    source: any NSDraggingSource
) -> NSDraggingSession
```

## Parameters 

`items`  

The dragging items. The frame property of each `NSDraggingItem` must be in the view’s coordinate system.

`event`  

The mouse-down event object from which to initiate the drag operation. In particular, its mouse location is used for the offset of the icon being dragged.

`source`  

An object that serves as the controller of the dragging operation. It must conform to the NSDraggingSource protocol and is typically the view itself or its NSWindow object.

## Return Value

The dragging session for the drag.

## Discussion

A basic drag starts by calling `beginDraggingSessionWithItems:event:source:`.

The caller can take the returned NSDraggingSession and continue to modify its properties. When the drag actually starts, the source is sent a draggingSession(_:willBeginAt:) message followed by multiple draggingSession(_:movedTo:) messages as the user drags.

Once the drag is ended or cancelled, the source receives a draggingSession(_:endedAt:operation:) method and the drag is complete.

## See Also

### Dragging Operations

func registerForDraggedTypes([NSPasteboard.PasteboardType])

Registers the pasteboard types that the view will accept as the destination of an image-dragging session.

func unregisterDraggedTypes()

Unregisters the view as a possible destination in a dragging session.

var registeredDraggedTypes: [NSPasteboard.PasteboardType]

The array of pasteboard drag types that the view can accept.

func shouldDelayWindowOrdering(for: NSEvent) -> Bool

Allows the user to drag objects from the view without activating the app or moving the window of the view forward, possibly obscuring the destination.


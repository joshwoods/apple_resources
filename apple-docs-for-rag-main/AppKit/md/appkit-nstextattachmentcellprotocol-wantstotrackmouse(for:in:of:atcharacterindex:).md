

- AppKit
- NSTextAttachmentCellProtocol
-  wantsToTrackMouse(for:in:of:atCharacterIndex:) 

Instance Method

# wantsToTrackMouse(for:in:of:atCharacterIndex:)

Allows an attachment to specify the events for which it tracks the mouse.

macOS

``` source
@MainActor
func wantsToTrackMouse(
    for theEvent: NSEvent,
    in cellFrame: NSRect,
    of controlView: NSView?,
    atCharacterIndex charIndex: Int
) -> Bool
```

**Required**

## Discussion

`theEvent` is the event in question that occurred in `cellFrame` inside `controlView`. `charIndex` is the index of the attachment character within the text. If wantsToTrackMouse() returns true, this method allows the attachment to decide whether it wishes to do so for particular events.

## See Also

### Responding to mouse events

func wantsToTrackMouse() -> Bool

Returns a Boolean value that indicates whether the attachment handles mouse events occurring over its image.

**Required**

func trackMouse(with: NSEvent, in: NSRect, of: NSView?, untilMouseUp: Bool) -> Bool

Handles a mouse-down event on the cell’s image, and optionally waits until a mouse-up event

**Required**

func trackMouse(with: NSEvent, in: NSRect, of: NSView?, atCharacterIndex: Int, untilMouseUp: Bool) -> Bool

Handles a mouse-down event on the image at the specified character position.

**Required**


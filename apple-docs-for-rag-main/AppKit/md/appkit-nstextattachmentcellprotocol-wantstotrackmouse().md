

- AppKit
- NSTextAttachmentCellProtocol
-  wantsToTrackMouse() 

Instance Method

# wantsToTrackMouse()

Returns a Boolean value that indicates whether the attachment handles mouse events occurring over its image.

macOS

``` source
@MainActor
func wantsToTrackMouse() -> Bool
```

**Required**

## Discussion

The default implementation of this method returns true. The NSView containing the cell should invoke this method before sending a trackMouse(with:in:of:untilMouseUp:) message.

For an attachment in an attributed string, if the attachment cell returns false, its attachment character should be selected rather than the cell being asked to track the mouse. This results in the attachment icon behaving as any regular glyph in text.

## See Also

### Responding to mouse events

func wantsToTrackMouse(for: NSEvent, in: NSRect, of: NSView?, atCharacterIndex: Int) -> Bool

Allows an attachment to specify the events for which it tracks the mouse.

**Required**

func trackMouse(with: NSEvent, in: NSRect, of: NSView?, untilMouseUp: Bool) -> Bool

Handles a mouse-down event on the cell’s image, and optionally waits until a mouse-up event

**Required**

func trackMouse(with: NSEvent, in: NSRect, of: NSView?, atCharacterIndex: Int, untilMouseUp: Bool) -> Bool

Handles a mouse-down event on the image at the specified character position.

**Required**


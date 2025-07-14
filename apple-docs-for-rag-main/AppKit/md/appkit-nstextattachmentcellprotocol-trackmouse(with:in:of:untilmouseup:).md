

- AppKit
- NSTextAttachmentCellProtocol
-  trackMouse(with:in:of:untilMouseUp:) 

Instance Method

# trackMouse(with:in:of:untilMouseUp:)

Handles a mouse-down event on the cell’s image, and optionally waits until a mouse-up event

macOS

``` source
@MainActor
func trackMouse(
    with theEvent: NSEvent,
    in cellFrame: NSRect,
    of controlView: NSView?,
    untilMouseUp flag: Bool
) -> Bool
```

**Required**

## Parameters 

`theEvent`  

The mouse-down event.

`cellFrame`  

The region of an NSTextView in which to track further mouse events.

`controlView`  

The view that received the event. Typically, this view is an NSTextView object and is focused.

`flag`  

A Boolean value that indicates whether to track the mouse until a mouse-up event occurs. If this parameter is false, stop tracking when a mouse-dragged event occurs outside of `cellFrame`.

## Return Value

true if the cell successfully finished tracking the mouse, or false if tracking was unsuccessful.

## Discussion

The NSTextAttachmentCell implementation of this method calls upon `aTextView`’s delegate to handle the event. If `theEvent` is a mouse-up event for a double click, the text attachment cell calls the textView(_:doubleClickedOn:in:at:) method of its delegate and returns true. Otherwise, depending on whether the user clicks or drags the cell, it sends the delegate a textView(_:clickedOn:in:at:): or a textView(_:draggedCell:in:event:at:) message and returns true. The NSTextAttachmentCell implementation returns false only if `flag` is false and the mouse is dragged outside of `cellFrame`. The delegate methods are invoked only if the delegate responds.

## See Also

### Related Documentation

func trackMouse(with: NSEvent, in: NSRect, of: NSView, untilMouseUp: Bool) -> Bool

Initiates the mouse tracking behavior in a cell.

func lockFocus()

Locks the focus on the view, so subsequent commands take effect in the view’s window and coordinate system.

Deprecated

### Responding to mouse events

func wantsToTrackMouse() -> Bool

Returns a Boolean value that indicates whether the attachment handles mouse events occurring over its image.

**Required**

func wantsToTrackMouse(for: NSEvent, in: NSRect, of: NSView?, atCharacterIndex: Int) -> Bool

Allows an attachment to specify the events for which it tracks the mouse.

**Required**

func trackMouse(with: NSEvent, in: NSRect, of: NSView?, atCharacterIndex: Int, untilMouseUp: Bool) -> Bool

Handles a mouse-down event on the image at the specified character position.

**Required**


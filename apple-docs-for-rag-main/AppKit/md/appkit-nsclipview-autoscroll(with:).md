

- AppKit
- NSClipView
-  autoscroll(with:) 

Instance Method

# autoscroll(with:)

Scrolls the clip view proportionally to `theEvent`’s distance outside of it.

macOS

``` source
@MainActor
func autoscroll(with event: NSEvent) -> Bool
```

## Discussion

`theEvent`‘s location should be expressed in the window’s base coordinate system (which it normally is), not the receiving NSClipView. Returns true if any scrolling is performed; otherwise returns false.

Never invoke this method directly; instead, the NSScrollView’s document view should repeatedly send itself autoscroll(with:) messages when the pointer is dragged outside the NSScrollView‘s frame during a modal event loop initiated by a mouse-down event. The NSView class implements autoscroll(with:) to forward the message to the receiver’s superview; thus the message is ultimately forwarded to the NSClipView.

## See Also

### Scrolling

func scroll(to: NSPoint)

Changes the origin of the clip view’s bounds rectangle to `newOrigin`.

func constrainScroll(NSPoint) -> NSPoint

Returns a scroll point adjusted from the proposed new origin, if necessary, to guarantee the view will lie within its document view.

Deprecated

func constrainBoundsRect(NSRect) -> NSRect

Constrains the bounds of the clip view while the user is magnifying and scrolling.


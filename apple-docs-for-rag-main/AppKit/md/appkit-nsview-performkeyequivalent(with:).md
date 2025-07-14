

- AppKit
- NSView
-  performKeyEquivalent(with:) 

Instance Method

# performKeyEquivalent(with:)

Implemented by subclasses to respond to key equivalents (also known as keyboard shortcuts).

macOS

``` source
@MainActor
func performKeyEquivalent(with event: NSEvent) -> Bool
```

## Parameters 

`event`  

The key-down event object representing a key equivalent.

## Return Value

true if `theEvent` is a key equivalent that the view handled, false if it is not a key equivalent that it should handle.

## Discussion

If the view’s key equivalent is the same as the characters of the key-down event `theEvent`, as returned by charactersIgnoringModifiers, the view should take the appropriate action and return true. Otherwise, it should return the result of invoking `super`‘s implementation. The default implementation of this method simply passes the message down the view hierarchy (from superviews to subviews) and returns false if none of the view’s subviews responds true.

## See Also

### Handling Events in the View

func acceptsFirstMouse(for: NSEvent?) -> Bool

Overridden by subclasses to return true if the view should be sent a mouseDown(with:) message for an initial mouse-down event, false if not.

func hitTest(NSPoint) -> NSView?

Returns the farthest descendant of the view in the view hierarchy (including itself) that contains a specified point, or `nil` if that point lies completely outside the view.

func isMousePoint(NSPoint, in: NSRect) -> Bool

Returns whether a region of the view contains a specified point, accounting for whether the view is flipped or not.

func rightMouseDown(with: NSEvent)

Informs the receiver that the user has pressed the right mouse button.

var mouseDownCanMoveWindow: Bool

A Boolean value indicating whether the view can pass mouse down events through to its superviews.

var inputContext: NSTextInputContext?

The text input context object for the view.


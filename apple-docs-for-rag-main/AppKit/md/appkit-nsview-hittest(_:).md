

- AppKit
- NSView
-  hitTest(\_:) 

Instance Method

# hitTest(\_:)

Returns the farthest descendant of the view in the view hierarchy (including itself) that contains a specified point, or `nil` if that point lies completely outside the view.

macOS

``` source
@MainActor
func hitTest(_ point: NSPoint) -> NSView?
```

## Parameters 

`point`  

A point that is in the coordinate system of the view’s superview, not of the view itself.

## Return Value

A view object that is the farthest descendent of `aPoint`.

## Discussion

This method is used primarily by an NSWindow object to determine which view should receive a mouse-down event. You’d rarely need to invoke this method, but you might want to override it to have a view object hide mouse-down events from its subviews. This method ignores hidden views.

## See Also

### Related Documentation

func convert(NSPoint, to: NSView?) -> NSPoint

Converts a point from the view’s coordinate system to that of a given view.

### Handling Events in the View

func acceptsFirstMouse(for: NSEvent?) -> Bool

Overridden by subclasses to return true if the view should be sent a mouseDown(with:) message for an initial mouse-down event, false if not.

func isMousePoint(NSPoint, in: NSRect) -> Bool

Returns whether a region of the view contains a specified point, accounting for whether the view is flipped or not.

func performKeyEquivalent(with: NSEvent) -> Bool

Implemented by subclasses to respond to key equivalents (also known as keyboard shortcuts).

func rightMouseDown(with: NSEvent)

Informs the receiver that the user has pressed the right mouse button.

var mouseDownCanMoveWindow: Bool

A Boolean value indicating whether the view can pass mouse down events through to its superviews.

var inputContext: NSTextInputContext?

The text input context object for the view.


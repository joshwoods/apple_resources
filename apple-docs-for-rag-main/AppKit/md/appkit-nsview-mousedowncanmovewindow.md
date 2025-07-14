

- AppKit
- NSView
-  mouseDownCanMoveWindow 

Instance Property

# mouseDownCanMoveWindow

A Boolean value indicating whether the view can pass mouse down events through to its superviews.

macOS

``` source
@MainActor
var mouseDownCanMoveWindow: Bool { get }
```

## Discussion

This property lets you determine the region by which a window can be moved. The default value of this property is false if the view is opaque; otherwise, it is set to true. Subclasses can override this property to return different values based on the event.

## See Also

### Handling Events in the View

func acceptsFirstMouse(for: NSEvent?) -> Bool

Overridden by subclasses to return true if the view should be sent a mouseDown(with:) message for an initial mouse-down event, false if not.

func hitTest(NSPoint) -> NSView?

Returns the farthest descendant of the view in the view hierarchy (including itself) that contains a specified point, or `nil` if that point lies completely outside the view.

func isMousePoint(NSPoint, in: NSRect) -> Bool

Returns whether a region of the view contains a specified point, accounting for whether the view is flipped or not.

func performKeyEquivalent(with: NSEvent) -> Bool

Implemented by subclasses to respond to key equivalents (also known as keyboard shortcuts).

func rightMouseDown(with: NSEvent)

Informs the receiver that the user has pressed the right mouse button.

var inputContext: NSTextInputContext?

The text input context object for the view.


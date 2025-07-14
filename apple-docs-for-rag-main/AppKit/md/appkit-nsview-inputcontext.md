

- AppKit
- NSView
-  inputContext 

Instance Property

# inputContext

The text input context object for the view.

macOS 10.6+

``` source
@MainActor
var inputContext: NSTextInputContext? { get }
```

## Discussion

The value of this property is `nil` when the view does not conform to the NSTextInputClient protocol.

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

var mouseDownCanMoveWindow: Bool

A Boolean value indicating whether the view can pass mouse down events through to its superviews.




- AppKit
- NSTextView
-  scrollableTextView() 

Type Method

# scrollableTextView()

macOS 10.14+

``` source
@MainActor
class func scrollableTextView() -> NSScrollView
```

## See Also

### Controlling text display

func setNeedsDisplay(NSRect, avoidAdditionalLayout: Bool)

Marks the receiver as requiring display.

var shouldDrawInsertionPoint: Bool

A Boolean value that determines whether the receiver should draw its insertion point.

func drawInsertionPoint(in: NSRect, color: NSColor, turnedOn: Bool)

Draws or erases the insertion point.

func drawBackground(in: NSRect)

Draws the background of the text view.

func setConstrainedFrameSize(NSSize)

Attempts to set the frame size as if by user action.

func cleanUpAfterDragOperation()

Releases the drag information still existing after the dragging session has completed.

func showFindIndicator(for: NSRange)

Causes a temporary highlighting effect to appear around the visible portion (or portions) of the specified range.

class func scrollableDocumentContentTextView() -> NSScrollView

class func scrollablePlainDocumentContentTextView() -> NSScrollView


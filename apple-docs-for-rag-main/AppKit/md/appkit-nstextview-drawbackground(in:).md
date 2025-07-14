

- AppKit
- NSTextView
-  drawBackground(in:) 

Instance Method

# drawBackground(in:)

Draws the background of the text view.

macOS

``` source
@MainActor
func drawBackground(in rect: NSRect)
```

## Parameters 

`rect`  

The rectangle in which to draw the background.

## Discussion

Subclasses can override this method to perform additional drawing behind the text.

## See Also

### Controlling text display

func setNeedsDisplay(NSRect, avoidAdditionalLayout: Bool)

Marks the receiver as requiring display.

var shouldDrawInsertionPoint: Bool

A Boolean value that determines whether the receiver should draw its insertion point.

func drawInsertionPoint(in: NSRect, color: NSColor, turnedOn: Bool)

Draws or erases the insertion point.

func setConstrainedFrameSize(NSSize)

Attempts to set the frame size as if by user action.

func cleanUpAfterDragOperation()

Releases the drag information still existing after the dragging session has completed.

func showFindIndicator(for: NSRange)

Causes a temporary highlighting effect to appear around the visible portion (or portions) of the specified range.

class func scrollableDocumentContentTextView() -> NSScrollView

class func scrollablePlainDocumentContentTextView() -> NSScrollView

class func scrollableTextView() -> NSScrollView




- AppKit
- NSTextView
-  setNeedsDisplay(\_:avoidAdditionalLayout:) 

Instance Method

# setNeedsDisplay(\_:avoidAdditionalLayout:)

Marks the receiver as requiring display.

macOS

``` source
@MainActor
func setNeedsDisplay(
    _ rect: NSRect,
    avoidAdditionalLayout flag: Bool
)
```

## Parameters 

`rect`  

The rectangle in which display is required.

`flag`  

A value of true causes the receiver to not perform any layout, even if this means that portions of the text view remain empty. Otherwise the receiver performs at least as much layout as needed to display `aRect`.

## Discussion

`NSTextView` overrides the `NSView` setNeedsDisplay(_:) method to invoke this method with a `flag` argument of false.

## See Also

### Controlling text display

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

class func scrollableTextView() -> NSScrollView


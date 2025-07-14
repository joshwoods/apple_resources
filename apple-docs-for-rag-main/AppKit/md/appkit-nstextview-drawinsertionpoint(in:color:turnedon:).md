

- AppKit
- NSTextView
-  drawInsertionPoint(in:color:turnedOn:) 

Instance Method

# drawInsertionPoint(in:color:turnedOn:)

Draws or erases the insertion point.

macOS

``` source
@MainActor
func drawInsertionPoint(
    in rect: NSRect,
    color: NSColor,
    turnedOn flag: Bool
)
```

## Parameters 

`rect`  

The rectangle in which to draw the insertion point.

`color`  

The color with which to draw the insertion point.

`flag`  

true to draw the insertion point, false to erase it.

## Discussion

The focus must be locked on the receiver when this method is invoked. You should not need to invoke this method directly.

## See Also

### Related Documentation

var backgroundColor: NSColor

The receiver’s background color.

func lockFocus()

Locks the focus on the view, so subsequent commands take effect in the view’s window and coordinate system.

Deprecated

var insertionPointColor: NSColor!

The color of the insertion point.

### Controlling text display

func setNeedsDisplay(NSRect, avoidAdditionalLayout: Bool)

Marks the receiver as requiring display.

var shouldDrawInsertionPoint: Bool

A Boolean value that determines whether the receiver should draw its insertion point.

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


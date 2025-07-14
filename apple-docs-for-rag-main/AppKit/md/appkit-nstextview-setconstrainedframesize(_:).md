

- AppKit
- NSTextView
-  setConstrainedFrameSize(\_:) 

Instance Method

# setConstrainedFrameSize(\_:)

Attempts to set the frame size as if by user action.

macOS

``` source
@MainActor
func setConstrainedFrameSize(_ desiredSize: NSSize)
```

## Parameters 

`desiredSize`  

The new desired size.

## Discussion

This method respects the receiver’s existing minimum and maximum sizes and by whether resizing is permitted.

## See Also

### Related Documentation

var minSize: NSSize

The receiver’s minimum size.

var isVerticallyResizable: Bool

A Boolean that controls whether the receiver changes its height to fit the height of its text.

var isHorizontallyResizable: Bool

A Boolean that controls whether the receiver changes its width to fit the width of its text.

var maxSize: NSSize

The receiver’s maximum size.

### Controlling text display

func setNeedsDisplay(NSRect, avoidAdditionalLayout: Bool)

Marks the receiver as requiring display.

var shouldDrawInsertionPoint: Bool

A Boolean value that determines whether the receiver should draw its insertion point.

func drawInsertionPoint(in: NSRect, color: NSColor, turnedOn: Bool)

Draws or erases the insertion point.

func drawBackground(in: NSRect)

Draws the background of the text view.

func cleanUpAfterDragOperation()

Releases the drag information still existing after the dragging session has completed.

func showFindIndicator(for: NSRange)

Causes a temporary highlighting effect to appear around the visible portion (or portions) of the specified range.

class func scrollableDocumentContentTextView() -> NSScrollView

class func scrollablePlainDocumentContentTextView() -> NSScrollView

class func scrollableTextView() -> NSScrollView


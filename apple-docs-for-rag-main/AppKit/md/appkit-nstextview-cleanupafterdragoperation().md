

- AppKit
- NSTextView
-  cleanUpAfterDragOperation() 

Instance Method

# cleanUpAfterDragOperation()

Releases the drag information still existing after the dragging session has completed.

macOS

``` source
@MainActor
func cleanUpAfterDragOperation()
```

## Discussion

Subclasses may override this method to clean up any additional data structures used for dragging. In your overridden method, be sure to invoke `super`’s implementation of this method.

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

func showFindIndicator(for: NSRange)

Causes a temporary highlighting effect to appear around the visible portion (or portions) of the specified range.

class func scrollableDocumentContentTextView() -> NSScrollView

class func scrollablePlainDocumentContentTextView() -> NSScrollView

class func scrollableTextView() -> NSScrollView


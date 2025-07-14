

- AppKit
- NSWindow
-  disableCursorRects() 

Instance Method

# disableCursorRects()

Disables all cursor rectangle management within the window.

macOS

``` source
@MainActor
func disableCursorRects()
```

## Discussion

Use this method when you need to do some special cursor manipulation and you don’t want the Application Kit interfering.

## See Also

### Managing Cursor Rectangles

var areCursorRectsEnabled: Bool

A Boolean value that indicates whether the window’s cursor rectangles are enabled.

func enableCursorRects()

Reenables cursor rectangle management within the window after a disableCursorRects() message.

func discardCursorRects()

Invalidates all cursor rectangles in the window.

func invalidateCursorRects(for: NSView)

Marks as invalid the cursor rectangles of a given view object in the window, so they’ll be set up again when the window becomes key.

func resetCursorRects()

Clears the window’s cursor rectangles and the cursor rectangles of the NSView objects in its view hierarchy.


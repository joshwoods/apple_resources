

- AppKit
- NSWindow
-  discardCursorRects() 

Instance Method

# discardCursorRects()

Invalidates all cursor rectangles in the window.

macOS

``` source
@MainActor
func discardCursorRects()
```

## Discussion

This method is invoked by resetCursorRects() to clear out existing cursor rectangles before resetting them. You shouldn’t invoke it in the code you write, but you might want to override it to change its behavior.

## See Also

### Managing Cursor Rectangles

var areCursorRectsEnabled: Bool

A Boolean value that indicates whether the window’s cursor rectangles are enabled.

func enableCursorRects()

Reenables cursor rectangle management within the window after a disableCursorRects() message.

func disableCursorRects()

Disables all cursor rectangle management within the window.

func invalidateCursorRects(for: NSView)

Marks as invalid the cursor rectangles of a given view object in the window, so they’ll be set up again when the window becomes key.

func resetCursorRects()

Clears the window’s cursor rectangles and the cursor rectangles of the NSView objects in its view hierarchy.


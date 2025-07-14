

- AppKit
- NSWindow
-  enableCursorRects() 

Instance Method

# enableCursorRects()

Reenables cursor rectangle management within the window after a disableCursorRects() message.

macOS

``` source
@MainActor
func enableCursorRects()
```

## See Also

### Managing Cursor Rectangles

var areCursorRectsEnabled: Bool

A Boolean value that indicates whether the window’s cursor rectangles are enabled.

func disableCursorRects()

Disables all cursor rectangle management within the window.

func discardCursorRects()

Invalidates all cursor rectangles in the window.

func invalidateCursorRects(for: NSView)

Marks as invalid the cursor rectangles of a given view object in the window, so they’ll be set up again when the window becomes key.

func resetCursorRects()

Clears the window’s cursor rectangles and the cursor rectangles of the NSView objects in its view hierarchy.




- AppKit
- NSWindow
-  resetCursorRects() 

Instance Method

# resetCursorRects()

Clears the window’s cursor rectangles and the cursor rectangles of the NSView objects in its view hierarchy.

macOS

``` source
@MainActor
func resetCursorRects()
```

## Discussion

Invokes discardCursorRects() to clear the window’s cursor rectangles, then sends resetCursorRects() to every `NSView` object in the window’s view hierarchy.

This method is typically invoked by the NSApplication object when it detects that the key window’s cursor rectangles are invalid. In program code, it’s more efficient to invoke invalidateCursorRects(for:).

## See Also

### Managing Cursor Rectangles

var areCursorRectsEnabled: Bool

A Boolean value that indicates whether the window’s cursor rectangles are enabled.

func enableCursorRects()

Reenables cursor rectangle management within the window after a disableCursorRects() message.

func disableCursorRects()

Disables all cursor rectangle management within the window.

func discardCursorRects()

Invalidates all cursor rectangles in the window.

func invalidateCursorRects(for: NSView)

Marks as invalid the cursor rectangles of a given view object in the window, so they’ll be set up again when the window becomes key.

